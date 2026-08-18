---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-2-0.html"
breadcrumb-title: ''
description: Consulte as notas de versão do plug-in Unity versão 2.2.0 para saber mais sobre novos recursos, aprimoramentos e correções de erros.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.2.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.2.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---


# Unity 2.2.0

## 2.2.0 Notas de versão

**data de lançamento: 1/10/2019**

### Plug-in de núcleo:

* Substance Engine atualizado
* Melhoria na estabilidade do código
* **Suporte ao Unity 2018.3**
* Suporte ao **.NET 4.x**
* Suporte a Substance Source em 2018.3
* o problema de coloração do Substance Source foi corrigido
* O gráfico e o material correspondente agora têm o mesmo nome de objeto
* Aprimoramentos adicionados na legibilidade da interface gráfica do Unity Pro
* Suporte adicionado para atribuições de saída de material
* Correção de um erro com manipulação de sRGB
* Correção de um erro em que um usuário podia excluir todas as instâncias de um gráfico
* Correção de um erro em que a tentativa de renderizar Substance ao alterar parâmetros em tempo de execução fazia com que apenas dois fossem renderizados por vez
* Ao importar um pacote que contém arquivos de Substance antigos, o plug-in agora permitirá que o usuário saiba que ele contém dados de Substance antigos e exclua os arquivos de pacote quando o Unity estiver tentando importá-los (isso é para que o usuário não tenha que excluir tudo manualmente se ele veio com falha)
* Adicionado um botão &#39;Sobre&#39; no menu Substance para mostrar informações de compilação relacionadas ao plug-in Substance
* Adição das dicas de ferramentas do mouse sobre a interface gráfica do Substance para mostrar os nomes dos parâmetros de Substance expostos
* Adicionados botões de navegação na interface gráfica do Substance para vincular ao Substance e aos materiais
* Adicionados novos ícones para o gráfico de Substance/material/texturas no Navegador de conteúdo
* Miniaturas de Substance atualizadas no navegador de conteúdo
* Removido o .mat da frente dos nomes de material do Substance
* Adicionada a capacidade de renomear materiais e gráficos de Substance
* Ao alterar a resolução do gráfico de Substance, o pop-up aplicar/reverter não será mais exibido, forçando o usuário a confirmar a alteração nesse momento
* Correção de um erro em que o processo de reflexo usava apenas a resolução de Substance padrão, em vez de uma definida pelo usuário
* Adicionado um aviso do mouse à interface gráfica do Substance que informa ao usuário se o espaço da cor está definido como Gama
* Funcionalidade alterada de instâncias de gráficos de Substance: agora os usuários podem criar instâncias de gráficos em um Substance sem serem solicitados a fornecer informações sobre cada instância criada na GUI de gráficos de Substance

### Scripts:

* Ocultamos algumas funções não destinadas ao suporte a scripts
* Função adicionada para duplicar instâncias do gráfico de Substance por meio do script: Duplicate()
* Função adicionada para consultar informações de entrada de procedimento via C#, retorna uma matriz de elementos &#39;InputProperties&#39;: GetInputProperties()
* Função adicionada para verificar se existe uma entrada em um gráfico, retorna true/false: HasInput(string inputName)
* Função adicionada para verificar se uma entrada visibleif está visível, retorna true/false: IsInputVisible(string inputName)
* O esquema de renderização foi recriado. Assim, RenderSubstancesAsync() foi descontinuado e alterado para graphName.RenderAsync()

## Problemas conhecidos:

**Plug-in Core Substance**

* O usuário deve desativar &#39;Ativar Bitcode&#39; no menu Configurações de Compilação no Xcode para compilar para o iOS
* As visualizações do objeto Substance no Navegador de conteúdo aparecem em preto quando o destino da compilação é definido como Android/iOS
* O botão Alpha e o controle deslizante de visualização do Mapa de mip estão ausentes na interface de textura não-Substance após a importação do plug-in Substance
* O usuário precisa usar poderes de dois para definir uma resolução de gráfico de Substance através de script
* Os materiais de Substance não são persistentes quando exportados/importados usando um pacote do Unity
* Os Substance não funcionam com pacotes de ativos
* Todos os ícones de visualização de Substance no Navegador de ativos mudam para o ícone Substance S após uma reimportação
* Renomear um gráfico de Substance que tenha um material na cena removerá esse material dos objetos em que ele é colocado
* (Somente Mac) Atualizar o plug-in no Mac remove materiais de Substance das pré-fabricações na cena|

**Script**

* O script não funciona em tempo de execução se o projeto estiver definido como x86 nas configurações de compilação
* Problemas ao usar o backend de script il2cpp com determinadas plataformas de compilação

**Live Link do Substance Painter**

* Criar um projeto após pintar com o Substance Live Link definirá a malha pintada de volta para um material padrão
* Canal AO não enviado com o link do Painter Live
* Malhas com vários materiais não funcionam no Unity Live Link
* A forma como o Unity LiveLink usa o SimpleJson entra em conflito com outras instâncias do SimpleJson em um projeto
