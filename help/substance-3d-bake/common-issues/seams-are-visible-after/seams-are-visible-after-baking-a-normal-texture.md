---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/seams-are-visible-after-baking-a-normal-texture.html"
breadcrumb-title: ''
description: Elimine as emendas visíveis nas texturas normais cozidas ajustando o preenchimento, a suavização de borda e o layout UV.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Seams are visible after baking a normal texture
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: As emendas ficam visíveis após assar uma textura normal
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# As emendas ficam visíveis após assar uma textura normal

>[!WARNING]
>
> **Problema**
> 
> As costuras de mapa normais são visíveis nas bordas UV da malha, mesmo após uma cozedura limpa.

>[!NOTE]
>
> **Explicação**
> 
> Mesmo depois de um bolo perfeito, costuras ainda podem ser visíveis. A principal razão é que uma informação de superfície aproximada normal em uma textura. Às vezes, a textura não tem precisão ou tem que compensar demais entre a geometria baixa e alta para ser precisa o suficiente. Em outra situação, a forma como a geometria é apresentada com seu mapa normal pode afetar a sua aparência.

>[!NOTE]
>
> **Solução**
> 
> Algumas soluções possíveis podem ser tentadas para reduzir a intensidade das emendas com mapas normais:
> 
> * Geralmente, os UVs não são alinhados aos pixels, o que leva à suavização e produz emendas. Consulte [esta página](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md) para obter mais informações.
>   * Aumentar a resolução da textura pode ser uma maneira de reduzir esse efeito.
>   * Alinhar as bordas UV aos pixels é outra maneira de reduzir esse efeito.
> * Aumente a configuração de **qualidade** do sombreador. A qualidade do sombreador pode afetar como os reflexos de specular são calculados. Se algumas Ilhas UV estiverem rotacionadas e esse parâmetro estiver muito baixo, ele poderá produzir emendas visíveis. Consulte [esta página](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/pbr-metal-rough-172818827.html) para obter mais informações.
