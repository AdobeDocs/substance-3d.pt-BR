---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/blender/substance-in-blender-overview.html"
breadcrumb-title: ''
description: Saiba mais sobre o complemento do Substance 3D para Blender e como importar e trabalhar com materiais do Substance em seus projetos.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > Substance in Blender Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance na visão geral do Blender
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---


# Substance na visão geral do Blender

## Visão geral do plug-in

O complemento do Substance 3D permite importar materiais do Substance para o Blender. Usando o painel Substance 3D, você pode gerenciar e personalizar os materiais de Substance em seu projeto a partir de um único local. O complemento gera mapas de textura a partir de arquivos .sbsar e os usa para criar um material de mesclagem. Essas texturas são atualizadas automaticamente quando os parâmetros de Substance são ajustados.

## Importação de um material de Substance

1. Clique no botão **Carregar** no painel do Substance 3D.
1. Na janela aberta, navegue até o local onde seus arquivos .sbsar estão armazenados e selecione um ou mais. Em seguida, clique no botão **Carregar material de Substance**.
1. Clique no ícone de esfera no painel Material para abrir o menu suspenso e selecionar o material do Substance. Isso atribuirá o material ao slot atual. Como alternativa, use o botão Aplicar no painel Substance 3D para atribuir o material em um novo slot de material que não substitua a atribuição atual.

>[!NOTE]
>
> Se o objeto não tiver materiais, o botão **Aplicar** anexará automaticamente o material do Substance.

![](../../../assets/blender-overview-steps.png)

## O painel Substance 3D

O painel Substance 3D é usado para gerenciar os materiais de Substance em um projeto e ajustar seus parâmetros individuais. A seção Parâmetros de gráfico tem controles para resolução de textura, divisão em blocos gráficos, aleatoriedade e predefinições. A seção Saídas tem controles para os formatos de imagem das texturas geradas. A seção Parâmetro de Substance é onde os parâmetros de Substance podem ser ajustados.

Para obter mais informações, consulte a página [Painel do Substance 3D](../../../3d-applications/blender/the-3d-panel/the-substance-3d-panel.md).

## Preferências

Comportamentos padrão e outras configurações podem ser ajustados nas preferências do complemento. A opção “Anexar automaticamente o material” pode ser habilitada para anexar automaticamente materiais Substance a objetos e substituir a atribuição de material atual. “Realçar automaticamente o material para os objetos selecionados” alterará o material realçado no painel Substance 3D se um objeto com esse material for selecionado. Ativar a opção “texturas de atualização automática de ciclos” permitirá que as texturas sejam atualizadas na Janela de visualização 3D ao usar a visualização de renderização de ciclos.

O Deslocamento pode ser ativado com a opção para Height na seção Saídas. Aqui você poderá também ajustar o formato do arquivo e a profundidade de bits de cada saída.

Para obter mais informações, consulte a página [Preferências](../../../3d-applications/blender/preferences/preferences.md).

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../../assets/blender-overview-preferences-1-v2.png)

</td>
<td style="border: 0;" valign="top">

![](../../../assets/blender-overview-preferences-2-v2.png)

</td>
<td style="border: 0;" valign="top">

![](../../../assets/blender-overview-preferences-3.png)

</td>
</tr>
</table>

## Encontre mais materiais sobre Substance

Milhares de materiais e outros ativos criados profissionalmente estão disponíveis para download na [Substance 3D Assets](https://helpx.adobe.com/substance-3d/unlisted/assets.html). Muitos outros ativos que foram compartilhados pela Comunidade gratuitamente podem ser encontrados na [Comunidade do Substance 3D](https://helpx.adobe.com/substance-3d/unlisted/community-assets.html)

## Comunidade

Para obter ajuda geral, feedback ou relatar defeitos, ingresse no canal #substance-blender-beta no [servidor Substance Discord](https://discord.com/invite/substance3d) ou nas [comunidades Adobe](https://community.adobe.com/t5/substance-3d-plugins/ct-p/ct-substance-3d-plugins?page=1&sort=latest_replies&lang=all&tabid=all&topics=label-blender).
