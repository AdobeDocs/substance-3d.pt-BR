---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/tiling-substance-ue4.html"
breadcrumb-title: ''
description: Texturas Substance de blocos no Unreal Engine 4 adicionando nós de coordenadas de Textura e parâmetros escalares aos materiais.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Tiling Substance - UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance de divisão em blocos gráficos - UE4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '77'
ht-degree: 0%

---


# Substance de divisão em blocos gráficos - UE4

Para cobrir uma textura do substance, você precisará adicionar um nó Coordenada de Textura e multiplicá-lo pelo parâmetro escalar.

<https://docs.unrealengine.com/latest/INT/Engine/Rendering/Materials/ExpressionReference/Coordinates/#texturecoordinate>

Para criar parâmetros para os blocos U e V, você pode usar um Acrescentar vetor e multiplicá-lo pelo TextCoord. Isso permite que você defina independentemente os valores dos ladrilhos U e V.

![](../../../../assets/tiling-3.png){width="800px"}
