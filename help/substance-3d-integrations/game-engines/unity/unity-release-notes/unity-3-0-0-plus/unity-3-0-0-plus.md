---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-3-0-0-plus.html"
breadcrumb-title: ''
description: Consulte as notas de versão do plug-in Unity versão 3.0.0 e posterior para saber mais sobre novos recursos e aprimoramentos.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 3.0.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 3.0.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '1384'
ht-degree: 0%

---


# Unity 3.0.0+

## Unity 3.12.0

<b>Adicionado/Atualizado:</b>

* Suporte ao conector do Substance 3D no Unity, habilitando a funcionalidade Enviar para para enviar ativos entre o Substance 3D Sampler e o Unity.
* Suporte para renomear e republicar gráficos .sbsar do Designer para o Unity, garantindo que as alterações feitas no Designer persistam quando o gráfico atualizado é reimportado para o plug-in do Unity.
* Documentação para compartilhamento de arquivos .sbsar entre projetos do Unity.
* Página de contribuição da comunidade para a documentação do plug-in Unity: https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/community-contributions.html.

<b>Corrigido:</b>

* Ocorreu um problema em que a miniatura do material na pasta de ativos do projeto do Unity não é atualizada após a republicação de um arquivo .sbsar, exibindo o material anterior em vez do atual.

## Unity 3.11.0

<b>Adicionado/Atualizado:</b>

* Desempenho aprimorado para projetos com mais de 1.000 gráficos de Substance, reduzindo significativamente os tempos de resposta da interface do usuário ao inspecionar arquivos sbsar na pasta Ativos.
* Adicionado um botão de redefinição para reverter os arquivos sbsar ao seu estado original, aprimorando a eficiência do fluxo de trabalho.
* Documentação atualizada com uma solução alternativa para o problema “Entradas de imagem bloqueadas para 8 bits”, disponível em: [Integrações do Substance 3D no Unity - Atualizando projetos e problemas conhecidos](../../../../game-engines/unity/upgrading-projects-known/upgrading-projects-known-issues.md).
* Documentação atualizada para solucionar o erro “Falha de asserção na expressão” encontrado ao navegar em pastas do painel no Unity: [Integrações do Substance 3D no Unity - Atualizando projetos e problemas conhecidos](../../../../game-engines/unity/upgrading-projects-known/upgrading-projects-known-issues.md).

<b>Corrigido:</b>

* Correção de um problema que causava a quebra do plug-in nas plataformas Linux.
* Correção de problemas de compatibilidade com o plug-in Unity na versão 2023.

## Unity 3.10.1

<b>Corrigido:</b>

* Correção de um problema em que o Substance Engine não era carregado devido a um problema com sbsario.dll no plug-in Substance 3D para Unity.

## Unity 3.10.0

<b>Adicionado/Atualizado:</b>

* Seção de comentários atualizada para a API RenderInstanceAsync no plug-in

<b>Corrigido:</b>

* Resolvido um problema de vazamento de memória no código C++ do plug-in, garantindo a recuperação completa da memória após o descarte de objetos.
* Correção de um problema no Linux em que a importação do pacote de plug-ins do Unity resultava em um erro “SubstanceException: um argumento inválido foi fornecido para a API”, agora permitindo a importação bem-sucedida de arquivos SBSAR.
* Correção de um problema em que SubstanceGraphSO.CurrentStatePreset não estava funcionando corretamente para carregar predefinições com um script de janela de editor personalizado no Unity. Um script corretivo agora está disponível em nossa página de documentação do Substance (HelpX): https://experienceleague.adobe.com/en/docs/substance-3d/ecosystem/game-engines/unity/substance-3d-for-unity-scripting/substance-3d-for-unity-scripting
* Correção de um erro em que as propriedades do gráfico desapareciam ao serem selecionadas novamente no editor de unidade.
* Resolvido o problema “Tipo gerenciado desconhecido referenciado” relacionado ao SubstanceGraphSO no plug-in Unity, aprimorando a compatibilidade e a funcionalidade nas plataformas Android, especialmente para o Unity 2022.1 e potencialmente em todas as versões do Unity.
* Correção de um problema em que a seleção “FORMATO NORMAL” na seção PARÂMETROS TÉCNICOS era exibida incorretamente como um campo de entrada de número, em vez da lista suspensa esperada com as opções DirectX e OpenGL.

## Unity 3.9.0

<b>Adicionado/Atualizado:</b>

* Os arquivos Sbsar agora podem ser arrastados e soltos no projeto. O objeto .sbsar pode ser aplicado a uma malha como esperado no Unity 2022.3.
* Documentação aprimorada para o plug-in.

<b>Corrigido:</b>

* Correção de um problema em que o plug-in Unity não funcionava no Android.
* Restrições de nomenclatura atendidas no plug-in Unity. Quando um nome de arquivo continha um “.”, o plug-in não carregava o arquivo corretamente.
* Correção de um problema em que desmarcar “Gerar todas as saídas” não excluía automaticamente a textura extra.
* Correção da importação incorreta de materiais SBSAR nos projetos padrão do Unity 2021.3. Agora, no projeto de modelo padrão, os materiais SBSAR podem ser importados para a pasta de ativos e aplicados a uma malha 3D sem erros.
* Correção da importação incorreta de materiais SBSAR em projetos HDRP do Unity 2021/2022. Agora, no projeto de modelo HDRP, os materiais SBSAR podem ser importados para a pasta de ativos e aplicados a uma malha 3D sem erros.
* Correção de um erro de compilação ao gerar a compilação do Android para produzir o APK: “Falha na compilação; consulte a saída de erro do compilador para obter detalhes.”
* Correção de um problema que causava falha no processo de compilação do projeto com erros no Windows.
* Correção de um problema que causava falha no processo do projeto de compilação com erros no Android: UnityEditor.BuildPlayerWindow+BuildMethodException.
* Resolvida a UnityException encontrada ao alterar as entradas do SubstanceGraph no tempo de execução. Anteriormente, chamar SubstanceRuntimeGraph.SetTexturesResolution e SubstanceRuntimeGraph.Render() levou o SubstanceGraph a renderizar resultados incorretos.
* Correção de um erro tipográfico no SubstanceEditorTools.cs.

## Unity 3.8.0

<b>Adicionado/Atualizado:</b>

* Suporte introduzido para parâmetros com visibilidade condicional (recurso Visible If).
* Atualizado o mecanismo de Substance para a versão 9.
* Documentação atualizada para solucionar um problema com NativeGraph.InRenderWork não funciona em um script de janela do editor personalizado. Mais detalhes podem ser encontrados aqui: [Substance 3D para Script de Unidade - Documentação de Classe](../../../../game-engines/unity/3d-for-unity-scripting/class-documentation/substanceruntime-class/substanceruntime-class.md)

<b>Corrigido:</b>

* Correção de um problema que afetava mapas normais em projetos Android.
* Correção de um erro em que arrastar um objeto sbsar para a exibição de cena fazia com que todos os objetos que passavam o mouse fossem substituídos por seus materiais pelo material do objeto sbsar.
* Correção de um erro que causava erro ao inspecionar um material marcado como Somente tempo de execução no modo Tempo de execução e ao abrir o Mapeamento de textura de saída.

## Unity 3.7.0

<b>Adicionado/Atualizado:</b>

* Suporte para predefinições incorporadas e externas
* Compatibilidade com o Unity 2022.2

<b>Corrigido:</b>

* Erro ao criar um novo gráfico para um arquivo sbsar usando o botão copiar gráfico: “Transferência recursiva inesperada de classe com script”
* Criação de pasta de material extra no Mac após reabrir um projeto
* A matriz SubstanceFileSO não é atualizada ao criar/excluir instâncias de gráfico
* Opções de entrada incorretas são exibidas ao duplicar um Substance
* Campos de rótulo vazios nas exportações de arquivos .sbsprs
* Erros durante a exportação/importação de predefinição no editor: EndLayoutGroup: BeginLayoutGroup deve ser chamado primeiro.

<b>Removido:</b>

* Seção Canais do Plug-in Unity devido à falta de valor do usuário

## Unity 3.6.0

<b>Adicionado/Atualizado:</b>

* A capacidade de tornar valores Int 4 individuais editáveis independentemente.

<b>Corrigido:</b>

* Problema em que os materiais retornavam ao estado anterior ao reabrir um projeto
* Um erro em que a mensagem “Nenhum gráfico encontrado” era exibida ao tentar modificar o gráfico de material
* Ocorreu um problema no qual os valores de entrada para o parâmetro Deslocamento de rotação no recurso Tamanho físico não eram alterados
* Problema em que instâncias de gráfico duplicadas tinham valores GraphID incorretos para entradas
* Ocorreu um problema em que o gerador de Substance não era inicializado corretamente no editor ao usar scripts do editor (janela personalizada do editor) para alterar um gráfico
* Um problema em que exportar um SubstanceGraphSO.CurrentStatePreset de um script de janela do editor personalizado exportava uma versão em cache do gráfico
* Ocorreu um problema no qual as alterações de parâmetro não foram salvas quando a janela do inspetor foi bloqueada
* Um problema em que a entrada manual do teclado na seção Deslocamento de posição das opções de Tamanho físico não tinha efeito no material no modo Editor
* Erro ao digitar manualmente valores de parâmetro no objeto SBSAR

## Unity 3.5.0

<b>Adicionado/Atualizado:</b>

* Suporte para que os usuários alterem como as texturas de saída são atribuídas ao material do Unity
* Compatibilidade de plug-in com a versão mais recente do Unity 2022.2

<b>Corrigido:</b>

* Erro de referência nula quando os materiais têm uma entrada Int4
* Erro com entradas Int4, o valor W é atribuído a Data2 em vez de Data3
* Erro de ortografia no nome da função “\_OcclusionStrength”

## Unity 3.4.0

<b>Adicionado/Atualizado:</b>

* Posicione os controles de deslocamento para traduzir a textura pela superfície no painel tamanho físico
* Links para baixar o Substance 3D Assets Adobe e o Substance Community Assets nas configurações do projeto

## Unity 3.3.0

<b>Adicionado/Atualizado:</b>

* O recurso de tamanho físico para HDRP, que permite a aplicação e dimensionamento de materiais de acordo com o tamanho real
* Interface para ativação de GPU nas configurações do projeto

<b>Removido:</b>

* graphIDs da maioria das chamadas de API

## Unity 3.2.1

<b>Corrigido:</b>

* O problema com a atualização do plug-in de 3.0.0 e 3.1.0 para a versão mais recente.

## Unity 3.2.0

<b>Adicionado/Atualizado:</b>

* Melhoria de desempenho na recompilação de scripts

<b>Corrigido:</b>

* A importação do ativo falhou no plug-in Unity ao importar materiais Sbsar personalizados
* Erro “ArgumentException: o valor não está dentro do intervalo esperado”
* Erro “ArgumentOutOfRangeException: o índice estava fora do intervalo”

## Unity 3.1.0

<b>Adicionado/Atualizado:</b>

* Melhoria de desempenho de 1,38 vezes para o Mac
* O mecanismo de GPU no Mac usa Metal em vez de OpenGL

<b>Corrigido:</b>

* Problema do Mac em que os canais R e B das texturas de saída serão invertidos

## Unity 3.0.0

<b>Adicionado/Atualizado:</b>

* Suporte ao Apple Silicon
* Novo tutorial do YouTube sobre como usar o plug-in
* Nova documentação de scripting

<b>Corrigido:</b>

* Erro na exibição do inspetor ao pressionar o botão aleatório várias vezes
* Entradas de textura nula quebrando atualizações de Substance
* Os alternadores “Gerar todas as saídas”, “Gerar mapas de mip” e “Somente tempo de execução” não funcionam
* Problemas com os Namespaces
* Erro de referência nula ao entrar no modo de reprodução com o ativo do gráfico selecionado
* Problema com HDRP e URP para a versão LTS 2021.3 mais recente do Unity ao usar materiais apenas em tempo de execução
