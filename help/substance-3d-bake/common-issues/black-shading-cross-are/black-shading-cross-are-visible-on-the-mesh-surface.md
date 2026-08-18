---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/black-shading-cross-are-visible-on-the-mesh-surface.html"
breadcrumb-title: ''
description: Corrija artefatos de sombreamento preto visíveis em superfícies de malha corrigindo o espaço tangente e os cálculos normais.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Black shading cross are visible on the mesh surface
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Cruz sombreamento preta é visível na superfície da malha
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---


# A cruz sombreamento preta é visível na superfície da malha

Artefatos de sombreamento preto aparecem em várias áreas da malha quando sob iluminação.

![](../../assets/black-shading-cross.jpg)


## Explicação

Uma cruz com sombreado preto geralmente significa que o mapa normal não corresponde à malha, geralmente porque a geometria da malha mudou ou foi calculada de uma forma diferente do cálculo realizado pelo padeiro. Por exemplo: a triangulação da malha é diferente entre o padeiro e o visor, que renderiza a malha e seu mapa normal.

## Solução

Verifique se o aplicativo que mostra a malha e seu mapa normal está sincronizado com a forma como a textura foi cozida. Isto implica:

* Verifique se o espaço tangente é idêntico entre o visualizador e o padeiro.
* Verifique se o formato Normal é idêntico entre a vista e o padeiro.
* Verifique se a triangulação é idêntica entre o visualizador e o padeiro. Consulte [esta página](../../guides/triangulating-before-bak/triangulating-before-baking.md) para obter mais informações.
