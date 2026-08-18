---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/blender/workflows.html"
breadcrumb-title: ''
description: Saiba como usar materiais de Substance com os ciclos do Blender e renderizadores Evee para diferentes fluxos de trabalho.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > Workflows
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Fluxos de trabalhos
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---


# Fluxos de trabalhos

## Trabalhar com ciclos

Por padrão, as alterações de parâmetro não são atualizadas automaticamente na janela de visualização 3D quando visualizadas na visualização de renderização Ciclos. Para ver as atualizações no modo de exibição de renderização Ciclos, habilite **Texturas de atualização automática de ciclos** em Preferências para forçar a atualização.

## Arquivos .sbsar multigraph

O complemento suporta arquivos .sbrar com vários gráficos de substância. Ao carregar um arquivo com vários gráficos, um novo menu suspenso Gráficos aparecerá no painel Substance 3D. Ao contrário de outras alterações de parâmetro, alternar gráficos não atualizará automaticamente o material. Por isso, o botão **Aplicar** deve ser usado para atribuir o material novamente depois de alterar gráficos.

>[!NOTE]
>
> Por padrão, o botão Aplicar adiciona o material em um novo slot sem substituir as atribuições de material anteriores. Remova materiais anteriores ou use o menu suspenso de materiais para reatribuir materiais recém-aplicados.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/blender-workflows-multigraphs?$png$&jpegSize=100&wid=168)

## Trabalhar com entradas de imagem

Ao usar um material de Substance que permita entradas de imagens personalizadas, um parâmetro de seleção de imagem no painel Substance 3D permitirá que você abra o navegador de arquivos de uma imagem (ícone de pasta) ou selecione uma imagem que já exista em seu projeto (ícone de imagem suspenso).

A preferência Exportar formato de imagem pode ser usada para salvar as entradas de imagem geradas dentro do Blender na pasta temporária. Consulte a página [Preferências](../../../3d-applications/blender/preferences/preferences.md)para obter mais detalhes.

![](../../../assets/blender-workflows-image-inputs-steps.png)

## Predefinições de Rede do Sombreador.

A predefinição de sombreador pode ser ajustada rapidamente por meio do menu suspenso na seção Saídas do painel Substance 3D. Essas predefinições de sombreador ajustam a maneira como as texturas da imagem são aplicadas. Ciclos/Seda Padrão usa o mapeamento de coordenadas de textura UV regular. As outras três predefinições de Projeção de ciclos/véspera usam o mapeamento de coordenadas de textura gerado para métodos de projeção de caixa, esfera ou cilindro.

A predefinição de sombreador padrão usada pelos materiais pode ser selecionada no complemento [Preferências](../../../3d-applications/blender/preferences/preferences.md).

![](../../../assets/2022-08-12-12-12-33-adobeexpress-1.gif)

## Filtragem e ajuste de saídas

A seção Saídas do painel Substance 3D também tem opções para filtrar as saídas. Três botões ao lado do menu suspenso predefinição de sombreador podem ser usados para filtrar por saídas habilitadas (marca de seleção), saídas de sombreador (esfera) e todas as saídas disponíveis (linhas).

As saídas podem ser habilitadas individualmente usando a caixa de seleção. Quando uma saída estiver habilitada, uma saída correspondente no grupo de nós de textura será criada. Se essa saída for suportada pelo nó de material Principled BSDF, ela será conectada automaticamente a ela. O Height se conectará a um nó de deslocamento e a Oclusão ambiente se combinará com a cor base em um nó MixRGB.\
O menu suspenso Formato de arquivo ao lado da marca de seleção pode ser usado para definir o tipo de arquivo no qual a textura de saída é salva.

Além disso, as preferências de saída de arquivo padrão podem ser alteradas no complemento [Preferências](../../../3d-applications/blender/preferences/preferences.md).

## Trocando materiais em objetos

Clique no ícone de esfera no painel de propriedades do material do Blender para abrir uma lista de materiais no seu projeto de mesclagem. Os materiais de Substance que foram criados no painel também aparecerão na lista. Selecionar um material dessa lista substituirá o material ativo nesse slot de material.

## Deslocamento

Deslocamento da malha de texturas suportado no renderizador de ciclos, mas não no Eevee. Para ver o deslocamento, certifique-se de que a saída do Height esteja ativada. O complemento definirá automaticamente a configuração de deslocamento do material como **Deslocamento e Relevo**. A exibição do material em um objeto agora mostrará deslocamento na visualização de renderização. A escala do deslocamento pode ser ajustada no painel de material ou no nó do deslocamento.

Para obter melhores resultados, use níveis de subdivisão mais altos ou malhas de alto polígono para materiais com detalhes de deslocamento complexos.
