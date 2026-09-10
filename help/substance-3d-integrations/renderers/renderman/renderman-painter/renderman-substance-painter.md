---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/renderman/renderman-substance-painter.html"
breadcrumb-title: ''
description: Exporte texturas de Substance Painter para o Renderman usando o material pxrSurface e as conversões de saída apropriadas.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Renderman > Renderman - Substance Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Renderman - Substance Painter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '116'
ht-degree: 1%

---


# Renderman - Substance Painter

O Substance Painter 2020.1 (6.1.0) oferece suporte a [&#128279;](https://docs.substance3d.com/display/SPDOC/Export)**Modelos de saída [pxrSurface**](https://rmanwiki.pixar.com/display/REN/PxrSurface) e pxrDisney.

![](../../../assets/renderman.png)

É recomendável usar **pxrSurface** para a Saída.

![](../../../assets/pxrsurface.png)

## Sombreador renderman (Maya - RM 23.1)

| Exportar Substance Painter | PxrSurface |
| --- | --- |
| CorDifusa | Difusão/Cor |
| Aspereza especular | Specular/aspereza principal |
| SpecularFaceColor | Specular/cor do rosto principal |
| Normal | Globals / Bump / PxrNormalMap → Orientação (Open GL) |
| Deslocamento | (canal vermelho ) PxrDispTransform (Resultado F) → (disp scalar) PxrDisplace (Out Color) → (Sombreador do Deslocamento) PxrSurfaceSG |
| GlowColor | Brilho/cor (ganho = 1,0) |
| Presença | Globais/Presença |

>[!NOTE]
>
> Os mapas que representam dados precisarão ser interpretados corretamente. Consulte a página [Gerenciamento de cores](../../../renderers/color-management/color-management.md)para obter mais informações.
