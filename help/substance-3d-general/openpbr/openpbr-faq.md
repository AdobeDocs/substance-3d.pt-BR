---
title: Perguntas frequentes
description: Encontre respostas para perguntas frequentes sobre OpenPBR e Substance 3D.
source-git-commit: a3ceb4df30f08099799bc2caecc5446d3832fc06
workflow-type: tm+mt
source-wordcount: '1424'
ht-degree: 0%

---


# OpenPBR Perguntas frequentes

## O modelo de OpenPBR

+++O que é OpenPBR e qual versão é compatível com o Painter?

OpenPBR é uma especificação de material aberto hospedada pela Academy Software Foundation, definindo um modelo de sombreamento padronizado projetado para funcionar de forma consistente entre os aplicativos. [A documentação da Painter tem mais informações sobre como usar o OpenPBR](https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/home).

+++

+++O que significa quando um aplicativo solicita “suporte ao OpenPBR” e como posso descobrir como um aplicativo específico oferece suporte a ele?

Não há um processo formal de certificação, portanto a solicitação pode significar coisas diferentes. Na prática, as implementações variam: algumas abrangem a especificação completa, outras apenas um subconjunto, deixando de fora recursos como filme fino, dispersão ou certos comportamentos subsuperficiais. Observe também que “suporte a MaterialX” e “suporte a OpenPBR” não são a mesma coisa; um aplicativo pode suportar um sem implementar totalmente o outro.

Para descobrir o que um aplicativo específico realmente suporta, use uma combinação de abordagens: verifique as notas de versão (o suporte é frequentemente adicionado de forma incremental); carregue o OpenPBR Sombreador Playground do ASWF e compare com uma renderização de referência para lacunas de superfície rapidamente; ou, para estúdios com investimento significativo em pipeline, pergunte diretamente ao fornecedor sobre os recursos suportados e seu roteiro.

+++

+++O OpenPBR pode garantir resultados idênticos em diferentes aplicativos e renderizadores?

Não totalmente, e isso é por design. O OpenPBR define um modelo de material compartilhado, mas a aparência final também é moldada por iluminação, algoritmos de renderização, gerenciamento de cores e o grau de conformidade de cada implementação com a especificação.

Na prática, maximizar essa garantia significa: exportar via USD com integração com o MaterialX; validar a viagem de ida e volta com antecedência usando o Playground de Sombreador de OpenPBR do ASWF em vez de no final da produção; confirmar os níveis de suporte de seus fornecedores para quaisquer recursos avançados que você usar; e concordar antecipadamente sobre quais recursos serão e não serão usados em materiais compartilhados. A portabilidade deve ser validada ativamente, e não presumida.

+++

+++Há materiais que o OpenPBR não possa representar com precisão?

Sim. OpenPBR é um modelo paramétrico. Parâmetros como rugosidade, metalidade e IOR abrangem a grande maioria dos casos de uso da produção, mas não podem replicar a precisão de formatos de material medido, como X-Rite AxF, que captura dados ópticos reais de uma amostra física. Para a produção geral, o OpenPBR de trabalho é bem adequado; para aplicações que exigem correspondência exata da amostra, um formato medido pode ser mais apropriado.

A tinta de carro é uma ilustração útil. É possível criar tinta de carro no OpenPBR com um par de advertências. O OpenPBR não inclui um sombreador de tinta de carro especializado, então pode ser insuficiente para certos usos da indústria automotiva. Além disso, depende simplesmente do tipo de tinta de carro — algumas tintas de carro sempre terão propriedades que estão fora do escopo de qualquer sombreador. Mas com esses pontos em mente, a tinta do carro mapeia naturalmente a arquitetura em camadas do OpenPBR.

+++

## Configuração e conversão

+++Preciso aprender OpenUSD ou MaterialX para usar OpenPBR?

Não. Para a maioria dos artistas, o OpenPBR é simplesmente o modelo de material incorporado às ferramentas que eles já usam. Substance 3D Painter, Maya 2025.3 e 3ds Max 2026 usam o OpenPBR como material padrão; trabalhar com ele significa apenas trabalhar com o sombreador padrão. O USD e o MaterialX somente se tornam relevantes quando os materiais precisam se mover entre aplicativos. Para workflows de aplicativo único, o suporte nativo é suficiente; para pipelines de vários DCC, o USD e o MaterialX fornecem a infraestrutura de intercâmbio, mas em grande parte nos bastidores.

Dito isso, o caminho de troca mais robusto para bibliotecas de materiais compartilhados é via USD com integração MaterialX, que fornece um recipiente padronizado, renderizador-agnóstico para descrições de materiais. Os fluxos de trabalho para exportar materiais como ativos independentes (sem um modelo associado, para uso em uma biblioteca compartilhada) ainda estão em desenvolvimento ativo e ainda não são totalmente compatíveis em todos os lugares. Antes de se comprometer com uma arquitetura de biblioteca que depende disso, valide seu pipeline específico em relação aos recursos atuais.

+++

+++Como crio um novo projeto de OpenPBR no Substance 3D Painter?

Um projeto criado sem um modelo usa o sombreador de OpenPBR por padrão. O sombreador de OpenPBR é agora a primeira opção na janela do novo projeto, substituindo o ASM. Modelos dedicados também estão disponíveis para fluxos de trabalho específicos (Anisotropia, Revestimento, Fuzz, Dispersão da subsuperfície) e a importação de um arquivo USD que contém um material de OpenPBR configurará o projeto automaticamente. Os projetos de amostra enviados com o Substance 3D Painter também foram atualizados para usar o fluxo de trabalho do OpenPBR e são um bom ponto de partida para se familiarizar com seu funcionamento na prática.

+++

+++Posso converter um projeto de Adobe Standard Material (ASM) existente em OpenPBR?

Não há conversão automática. Os projetos existentes do ASM mantêm o sombreador atual quando abertos e os modelos do ASM permanecem disponíveis para novos projetos.

Para migrar manualmente para o OpenPBR, selecione o sombreador do OpenPBR na janela Configurações do Sombreador e adicione os canais de OpenPBR relevantes por meio das Configurações do conjunto de texturas > Adicionar ou remover canais. Depois disso, revise as camadas existentes para garantir que o conteúdo esteja direcionado aos canais desejados.

+++

+++Meus sombreadores personalizados precisam ser atualizados para o OpenPBR?

Não — os shaders personalizados existentes continuam funcionando, pois as bibliotecas de sombreador relevantes são descontinuadas em vez de removidas. No entanto, é recomendável migrar para as novas bibliotecas de sombreador; elas são mais limpas e mais fáceis de trabalhar. Consulte o log de alterações do API de sombreamento no menu Ajuda para obter detalhes.

+++

## Uso no aplicativo

+++Com tantos parâmetros disponíveis no OpenPBR, onde devo focar minha atenção?

Comece simples. Para a maioria das superfícies opacas, Cor de base, aspereza do Specular e metalidade respondem pela maioria das diferenças visíveis entre os materiais. Adicione IOR se a refletividade precisa for importante; refine a cor do Specular se o material tiver uma tonalidade de ângulo de pastagem. Permita transmissão, subsuperfície, revestimento, difusão, filme fino e dispersão somente quando tiver um motivo claro e orientado por referência para fazer isso, uma vez que cada canal adicional adiciona complexidade e potencial custo de renderização. Ocultar ou recolher grupos de parâmetros não utilizados mantém o foco do espaço de trabalho e reduz o risco de efeitos não intencionais.

+++

+++Eu tenho um mapa da aspereza — devo conectá-lo à Aspereza da Difusão base ou Aspereza do Specular?

Aspereza do specular: controla a nitidez do reflexo e é o equivalente direto da entrada de aspereza em outros fluxos de trabalho de PBR. A aspereza da Difusão base é um parâmetro especializado separado que afeta somente a dispersão difusa. Para a maioria dos fluxos de trabalho, ela pode permanecer em seu padrão.

+++

+++Por que mudar a Cor de base não tem efeito quando estou usando dispersão subsuperficial?

Há uma “hierarquia de prioridade” que determina quanta influência cada parâmetro tem sobre a aparência final do material. Curtir:

* A metalidade vem em primeiro lugar: quando a metalidade = 1, as partes da subsuperfície e da transmissão são desativadas.
* O Peso da Transmissão vem em seguida: se o Peso da Transmissão=1, a Subsuperfície estará ausente.
* O peso da subsuperfície vem depois disso.
* A Cor de base de Difusão vem por último: a base difusa só contribui quando nenhuma das anteriores está definida como 1.

Portanto, no exemplo mencionado, se a Espessura da subsuperfície for definida como 1 (seu valor máximo), ela controlará toda a aparência. Alterar o valor de Cor de base não tem efeito porque a Difusão base não faz essencialmente nenhuma contribuição. Por outro lado, se a Metalidade for definida com o valor máximo de 1, a alteração dos valores de Peso da transmissão, Peso da subsuperfície e Cor de base da Difusão não terá nenhum efeito na aparência final do material. Transmissão, Subsuperfície e Difusões são todos dielétricos (não-metálicos), portanto, definir a Metalidade como 1 é remover qualquer contribuição não-metálica.

+++

+++Por que a transmissão se comporta inesperadamente? Por exemplo, por que minha malha aparece muito escura quando eu a ativo?

O culpado mais comum é a Profundidade de transmissão sendo definida muito baixa. Esse parâmetro define a distância em que a luz viaja antes que a cor de transmissão atinja a saturação total; em valores baixos, até mesmo a geometria fina parece escura e densa. Aumente-o para corresponder à escala física aproximada do objeto. Se o material então parece muito claro, ajuste a Cor de transmissão e a Profundidade juntas para encontrar o equilíbrio certo.

A dispersão pode adicionar uma camada adicional de complexidade. A cor de transmissão não é um matiz simples; seu efeito depende da distância em que a luz viaja pelo objeto, controlado pela Profundidade de transmissão. A Cor de dispersão, por sua vez, controla uma luz de jornada separada que pode ser levada - refletindo no interior do material em vez de passar diretamente. Como a dispersão é direcional, o resultado também muda dependendo de onde a fonte de luz está colocada. Ajustar um sem considerar o outro é uma fonte comum de resultados inesperados.

+++

+++Eu ativei o filme fino, mas não consigo ver nenhum efeito. O que estou perdendo?

Verifique o valor do Thickness primeiro. Contraintuitivamente, valores mais finos produzem uma iridescência mais visível — a maioria dos efeitos ocorre entre 0 e 1 micrômetro. Se o efeito ainda for sutil, ajuste a IOR, que altera a intensidade e a cor da interferência. Confirme também se a Espessura da película fina está acima de zero.

+++
