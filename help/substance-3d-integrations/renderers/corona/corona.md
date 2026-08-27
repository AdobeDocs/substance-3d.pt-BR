---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/corona.html"
breadcrumb-title: ''
description: Use materiais de Substance com o renderizador Corona no 3ds Max usando o fluxo de trabalho Specular/Textura reluzente e os mapas necessários.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Corona
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Corona
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 1%

---


# Corona

Para renderizar com o Corona, você pode usar mapas exportados do Substance Painter ou o plug-in Substance. Corona está usando o fluxo de trabalho Specular/Textura reluzente com um mapa 1/IOR. Você precisará dos seguintes mapas:

* Difusão
* Reflexo (Specular)
* Textura reluzente
* 1/IOR (Convertido)

O mapa 1/IOR só pode ser convertido do fluxo de trabalho metálico/rugosidade, que é o fluxo de trabalho padrão em Substance Designer e Substance Painter.

1. Exporte mapas de Substance Painter usando a predefinição Corona.
1. Para Substance personalizados, você pode usar o nó convertido basecolor\_metallic\_roughness definido para a predefinição Vray para criar as saídas personalizadas.
1. Para o 3ds Max e o Cinema 4D, você usa um material Corona em camadas para manipular materiais metálicos e dielétricos e ignorar a necessidade de converter um mapa 1/IOR.

## Sumário

* [Corona para 3ds Max](../../renderers/corona/corona-for-3ds-max/corona-for-3ds-max.md)
* [Corona - Substance Painter](../../renderers/corona/corona-painter/corona-substance-painter.md)
