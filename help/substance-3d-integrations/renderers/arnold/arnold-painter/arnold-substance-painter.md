---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/renderers/arnold/arnold-substance-painter.html"
breadcrumb-title: ''
description: Use modelos de saída de Substance Painter para o renderizador Arnold com material aiStandard para renderização baseada fisicamente.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Arnold > Arnold - Substance Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Arnold - Substance Painter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 3%

---


# Arnold - Substance Painter

O Substance Painter 2020.1 (6.1.0) vem com [Modelos de saída](https://experienceleague.adobe.com/pt-br/docs/substance-3d-painter/using/getting-started/export/output-templates/export-presets) para Arnold usando o [material aiStandard](https://docs.arnoldrenderer.com/display/A5AFMUG/Standard+Surface).

![](../../../assets/arnold-export.png){width="800px"}

## Sombreador padrão Arnold (Arnold 5 e superior)

| Exportar Substance Painter | Arnold AiStandardSurface |
| --- | --- |
| BaseColor | Base / Cor |
| Rugosidade | Specular / Aspereza |
| Metalicidade | Base / Metalidade |
| Normal | (**Maya**) Geometry/ Bump Mapping / bump2d (Use como normais de Espaço tangente) (**3ds** **Max**) Bitmap → Normal |
| Altura | (**Maya**) Deslocamento Sombreador / deslocamento (**3ds** **Max**) Modificador de objeto → Arnold Propriedades → Deslocamento → Usar Mapa |
| Emissivo | Emissão/Cor (Peso da Emissão = 1,0) |
| Nível de anisotropia (não incluído no Modelo de saída Arnold padrão) | (**Maya**) Casaco/Anisotropia (**3ds** **Max**) Casaco/Anisotropia |
| Nível de anisotropia (não incluído no Modelo de saída Arnold padrão) | (**Maya**) Revestimento/Rotação (**3ds** **Max**) Revestimento/Rotação |

>[!NOTE]
>
> Os mapas que representam dados precisarão ser interpretados corretamente. Consulte a página [Gerenciamento de cores](../../../renderers/color-management/color-management.md)para obter mais informações.
