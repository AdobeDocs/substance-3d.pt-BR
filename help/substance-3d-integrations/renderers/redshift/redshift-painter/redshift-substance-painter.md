---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/renderers/redshift/redshift-substance-painter.html"
breadcrumb-title: ''
description: Exporte texturas de Substance Painter para o renderizador Redshift usando modelos de saída e configurações de material adequadas.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Redshift > Redshift - Substance Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Redshift - Substance Painter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '142'
ht-degree: 2%

---


# Redshift - Substance Painter

O Substance Painter 2020.1 (6.1.0) oferece suporte a [Modelos de saída](https://docs.substance3d.com/display/SPDOC/Export) do Redshift para metal/aspereza (rsMaterial). Você pode simplesmente exportar usando o modelo Redshift para produzir texturas compatíveis com os materiais do Redshift.

![](../../../assets/rs-export.png)

## Configuração de material do Redshift

| Exportar Substance Painter | Material do Redshift |
| --- | --- |
| Cor | Difusa/colorida |
| Rugosidade | Reflexo/aspereza (BRDF = GGX) |
| Metalicidade | Reflexo/Metalidade (Tipo Fresnel = Metalidade) |
| Normal | Geral / Bump Map / rsBumpMap (Tipo de mapa de entrada = Espaço tangente normal - Escala de Height = 1,0) |
| DisplaceHeightField | Deslocamento Shader / rsDisplacement TextMap (Codificação de mapa = Campo de Height) |
| CorDeEmissão | Geral/Emissão (Peso da Emissão = 1,0) |

>[!NOTE]
>
> Os mapas que representam dados precisarão ser interpretados corretamente. Consulte a página [Gerenciamento de cores](../../../renderers/color-management/color-management.md)para obter mais informações.

## Exemplo do Maya/Redshift

![](https://helpx-prod.scene7.com/is/image/HelpxProd/maya-example?$pjpeg$&jpegSize=300&wid=1583){width="800px"}
