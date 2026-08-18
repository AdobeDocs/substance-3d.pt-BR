---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/working-with-bump-offset-parallax-ue4.html"
breadcrumb-title: ''
description: Use o mapeamento de deslocamento de relevo com materiais de Substance no Unreal Engine 4 para criar ilusão de profundidade e detalhes de superfície.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Working with Bump Offset (Parallax) - UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Trabalhando com deslocamento de relevo (paralaxe) - UE4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---


# Trabalhando com deslocamento de relevo (paralaxe) - UE4

O mapeamento de **Deslocamento de relevo** dá a uma superfície a ilusão de profundidade, modificando as coordenadas UV de forma criativa para ajudar a deslocar ainda mais os texels da superfície do objeto, dando a ilusão de que a superfície tem mais detalhes do que realmente tem. Neste exemplo de “Como fazer”, abordaremos não apenas como você pode encontrar a expressão de material de deslocamento de relevo, mas também como você pode utilizar o nó Deslocamento de relevo em seus materiais.

<https://docs.unrealengine.com/latest/INT/Engine/Rendering/Materials/HowTo/BumpOffset/>

Para usar a saída do height, você precisa clicar duas vezes na Saída na Instância do Substance Fatory para criar o height. O height não é ativado por padrão. Em seguida, você pode arrastar a saída dessa height para o material.

![](../../../../assets/height-1.png){width="600px"}

Crie um nó de deslocamento de relevo e, em seguida, conecte o canal Vermelho do height ao Height. Em seguida, você pode alimentar um TextCoord na entrada de Coordenada do deslocamento de relevo. Finalmente, a saída do deslocamento de relevo é conectada à entrada UV para todas as texturas de Substance.

![](../../../../assets/bump.png){width="800px"}
