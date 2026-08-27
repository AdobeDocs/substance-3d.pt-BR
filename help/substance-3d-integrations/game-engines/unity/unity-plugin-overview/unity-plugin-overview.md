---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/game-engines/unity/unity-plugin-overview.html"
breadcrumb-title: ''
description: Saiba mais sobre o plug-in do Substance 3D para Unity, incluindo suporte à versão, recursos e recursos de integração.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Plugin Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Visão geral do plug-in Unity
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---


# Visão geral do plug-in Unity

## Suporte à versão do Unity

O plug-in Adobe Substance 3D para Unity versão 3.0.0 atualmente suporta Unity 2020 LTS e superior.

## Baixando o pacote do Substance

1. O Plug-in pode ser baixado do Repositório de Ativos do Unity: <https://assetstore.unity.com/packages/tools/utilities/substance-3d-for-unity-beta-213208>

## Importação de um material de Substance

1. Clique com o botão direito do mouse na janela Projeto e escolha Importar ativo ou arraste o Material do Substance que deseja importar para o painel de visualização do projeto.
1. Procure o material de Substance que deseja importar. Os materiais do Substance têm a extensão de arquivo “.sbsar”.
1. O material do Substance será importado para seu projeto do Unity.

   1. O ativo sbsar criará um arquivo de importação principal e uma pasta contendo as texturas de saída e um material gerado do Unity.
1. Em seguida, você pode arrastar e soltar o material em uma malha na visualização Cena e editar os parâmetros no Inspetor.

   ![](../../../assets/window-overview.png){width="1000px"}

>[!NOTE]
>
> **Conversão de Mapa normal**
> 
> O plug-in Substance do Unity converte automaticamente o DirectX em OpenGL. Ao usar materiais de [Substance Source](https://source.substance3d.com/), não é necessário alterar a orientação normal para OGL. Se você estiver criando seu próprio material em Substance Designer, certifique-se de trabalhar com o sombreador de DirectX padrão, pois o plug-in lidará com a conversão normal automaticamente. Para obter mais informações, consulte Trabalhando com normais no Unity.

## Alterando Parâmetros

Os parâmetros e as resoluções podem ser definidos na janela Inspetor. Consulte [Alterando Parâmetros](../../../game-engines/unity/changing-parameters/changing-parameters.md).

[unity\_tweaking\_parameters.mp4](https://helpx.adobe.com/content/dam/help/en/substance-3d/documentation/download/attachments/186056716/unity-tweaking-parameters.mp4)

## Suporte ao Pipeline de Renderização do Unity

O plug-in do Substance 3D é compatível com HDRP e URP. Mais informações estarão disponíveis em breve.

## Tutorial sobre como
