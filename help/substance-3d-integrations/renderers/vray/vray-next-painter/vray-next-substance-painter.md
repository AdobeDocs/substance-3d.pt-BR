---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/renderers/vray/vray-next-substance-painter.html"
breadcrumb-title: ''
description: Exporte texturas de Substance Painter para o renderizador V-Ray Next usando modelos de saída e configurações adequadas de fluxo de trabalho.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Vray > Vray Next - Substance Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Variar Próximo - Substance Painter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 3%

---


# Variar Próximo - Substance Painter

O Substance Painter 2020.1 (6.1.0) vem com sombreadores [VrayMtl](https://docs.chaosgroup.com/display/VRAY4MAYA/VRayMtl) para os fluxos de trabalho metálicos e de specular. Você pode [configurar seu projeto Substance Painter](https://docs.substance3d.com/display/SPDOC/Project+Creation) usando o **modelo VrayMtl**, que configurará seu sombreador de visor.

![](../../../assets/template-16.jpg)

Em Configurações do sombreador, você pode configurar o sombreador Vray para trabalhar com VrayMtl.

>[!NOTE]
>
> Se o seu projeto foi configurado para usar o [UV Tile UDIM Legacy](https://helpx.adobe.com/br/substance-3d/unlisted/documentation/spdoc/uv-tile-udim-legacy-144310352.html). Use o modelo de saída UDIM Vray Next.

![](../../../assets/vray-mtl-shader.png){width="800px"}

Para exportar texturas para renderização em Vray Próximo, escolha o Modelo de saída de Mtl Vray.

![](../../../assets/template-project.jpg){width="800px"}

## Vray Material (Vray Next - Metálico/Aspereza)

| Exportar Substance Painter | VRayMtl |
| --- | --- |
| BaseColor | Cor Difusa (**Maya**) (Quantidade = 1,0) (**3ds Max**) |
| Rugosidade | (**Maya**) Reflexão / Aspereza (BRDF = GGX) + (Usar aspereza habilitada)(**3ds Max**) Aspereza → BRDF/ Usar GGX e habilitar Usar aspereza |
| Metálico | (**Maya**) Reflexão/Metalidade (**3ds Max**) Metalidade |
| Normal | (**Maya**) Mapeamento de Relevo e Normal / Mapa (Tipo de Mapa = Normal no Espaço Tangente)(**3ds** **Max**) Bitmap → Normal |
| Altura | (**Maya**) Deslocamento Shader / deslocamento (**3ds** **Max**) Modificador de objeto → VrayDisplacementMod → Mapa de texto |
| Emissivo | Autoiluminação |
| Transmissivo | (**Maya**) Espalhamento de subsuperfície / Cor de transparência (**3ds Max**) Translucidez → Cor do verso |
| AnisotropyAngle | Rotação de Anisotropia/Anisotropia (**Maya**) (**3ds** **Max**) BRDF/Rotação |
| AnisotropyLevel | (**Maya**) Anisotropia/Anisotropia (**3ds Max**) BRDF/Ângulo |

## Material Vray (Vray Próximo - Specular/Textura reluzente

| Exportar Substance Painter | VRayMtl |
| --- | --- |
| Difusão | Cor Difusa (**Maya**) (Quantidade = 1,0) (**3ds Max**) |
| Especular | (**Maya**) Reflexo / Reflexo Cor (Quantidade = 1,0) (**3ds Max**) Refletir |
| Textura reluzente | (**Maya**) Reflexão / Aspereza (BRDF = GGX) + (Usar aspereza habilitada)(**3ds Max**) Textura reluzente → BRDF / Usar GGX e habilitar Usar glossiness |
| Normal | (**Maya**) Mapeamento de Relevo e Normal / Mapa (Tipo de Mapa = Normal no Espaço Tangente)(**3ds** **Max**) Bitmap → Normal |
| Altura | (**Maya**) Deslocamento Shader / deslocamento (**3ds** **Max**) Modificador de objeto → VrayDisplacementMod → Mapa de texto |
| Emissivo | Autoiluminação |
| Transmissivo | (**Maya**) Espalhamento de subsuperfície / Cor de transparência (**3ds Max**) Translucidez → Cor do verso |
| AnisotropyAngle | Rotação de Anisotropia/Anisotropia (**Maya**) (**3ds** **Max**) BRDF/Rotação |
| AnisotropyLevel | (**Maya**) Anisotropia/Anisotropia (**3ds Max**) BRDF/Ângulo |

>[!NOTE]
>
> Os mapas que representam dados precisarão ser interpretados corretamente. Consulte a página [Gerenciamento de cores](../../../renderers/color-management/color-management.md)para obter mais informações.

Este exemplo mostra a viewport Substance Painter usando o sombreador Vray Metallic/Roughness e a renderização Vray usando Maya.

![](../../../assets/vray-maya.jpg){width="800px"}
