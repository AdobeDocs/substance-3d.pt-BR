---
helpx_url: "https://helpx.adobe.com/br/substance-3d-bake/common-issues/seam-visible-on-every-face.html"
breadcrumb-title: ''
description: Corrija as emendas visíveis em cada face verificando o desembrulho UV, os grupos de suavização e os problemas de topologia de malha.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Seam visible on every face
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Costura visível em cada rosto
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---


# Costura visível em cada rosto

>[!WARNING]
>
> **Problema**
> 
> Uma costura é visível em algumas bordas da geometria, mesmo se não houver emendas UV presentes:
> 
> ![](../../assets/seam-every-face.jpg)

>[!NOTE]
>
> **Explicação**
> 
> Se não estiver usando uma [gaiola](https://helpx.adobe.com/br/substance-3d/unlisted/documentation/bake/cage-projection-172822982.html), o processo de cozimento iniciará raios na direção dos normais de vértice da malha de baixo-polígono. Se cada normais de vértice são divididos (o que significa que cada face não compartilha os mesmos normais de vértice que a face vizinha) os raios não serão enviados na mesma direção nas bordas. Isso resulta em divisão porque as informações em cada lado das bordas são diferentes.
> 
> Esse problema também é agravado pela suavização, conforme explicado em [esta página](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md).

>[!NOTE]
>
> **Solução**
> 
> Apenas duas soluções são possíveis aqui:
> 
> * Use uma [gaiola](https://helpx.adobe.com/br/substance-3d/unlisted/documentation/bake/cage-projection-172822982.html) para controlar a direção do raio em vez de deixar que o padeiro o calcule a partir da geometria de baixo-polígono.
> * Mescle os normais de vértice da malha de baixo polígono juntos (suavize-os / aplique um grupo de suavização comum).
