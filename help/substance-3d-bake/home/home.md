---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/home.html"
breadcrumb-title: ''
description: Saiba como usar o Substance Bakers para calcular informações baseadas em malha em arquivos de textura e aprimorar o fluxo de trabalho de texturização.
helpx_creative_field: ""
helpx_description: bakers > Home
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Panificadores Substance
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 13%

---


# Panificadores Substance

<table>
<tr style="border: 0;">
<td width="41.60%" style="border: 0;" valign="top">

Os <b>Substance Bakers</b> são um conjunto de ferramentas de algoritmo avançado para computar informações baseadas em malha em arquivos de textura. Eles podem ser usados por qualquer artista com uma malha 3D para aproveitar os métodos avançados de texturização. Fazer bake é um processo no núcleo do fluxo de trabalho do software Substance para oferecer<b> ferramentas poderosas</b> e <b>texturização automatizada</b>.

Esta documentação aborda os <b>fundamentos do faço bake</b> e os <b>problemas comuns</b> e os erros que podem ser encontrados ao lidar com este processo.

</td>
<td width="58.30%" style="border: 0;" valign="top">

![](../assets/optim-baker-home.png){width="400px"}

</td>
</tr>
</table>

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

## Introdução

* [O que é assar?](../getting-started/what-is-baking/what-is-baking.md)
* Fazer bake por:
  * [Substance 3D Painter](../getting-started/software-interface/3d-painter/substance-3d-painter.md)
  * [Substance 3D Designer](../getting-started/software-interface/3d-designer/substance-3d-designer.md)
  * [Substance 3D Automation Toolkit](../getting-started/software-interface/3d-automation-toolkit/substance-3d-automation-toolkit.md)
* [Disponibilidade por software](../getting-started/availability-per-software/availability-per-software.md)
* [Software 3D compatível](../getting-started/compatible-3d-software/compatible-3d-software.md)
* [Tutorials](../getting-started/tutorials/tutorials.md)

</td>
<td style="border: 0;" valign="top">

### Configurações de preparadores

* [Parâmetros comuns](../bakers-settings/common-parameters/common-parameters.md)
* [Oclusão de ambiente](../bakers-settings/ambient-occlusion/ambient-occlusion.md)
* [Oclusão ambiente da malha](../bakers-settings/ambient-occlusion-from/ambient-occlusion-from-mesh.md)
* [Normais tortos da malha](../bakers-settings/bent-normals-from-mesh/bent-normals-from-mesh.md)
* [Mapa de cores da malha](../bakers-settings/color-map-from-mesh/color-map-from-mesh.md)
* [Converter UV para SVG](../bakers-settings/convert-uv-to-svg/convert-uv-to-svg.md)
* [Curvatura](../bakers-settings/curvature/curvature.md)
* [Curvatura da malha](../bakers-settings/curvature-from-mesh/curvature-from-mesh.md)
* [Curvatura da malha (descontinuado)](../bakers-settings/curvature-from-mesh-dep/curvature-from-mesh-deprecated.md)
* [Mapa de altura da malha](../bakers-settings/height-map-from-mesh/height-map-from-mesh.md)
* [Mapa normal da malha](../bakers-settings/normal-map-from-mesh/normal-map-from-mesh.md)
* [Máscara de opacidade da malha](../bakers-settings/opacity-mask-from-mesh/opacity-mask-from-mesh.md)
* [Posição](../bakers-settings/position/position.md)
* [Mapa de posição da malha](../bakers-settings/position-map-from-mesh/position-map-from-mesh.md)
* [Mapa de espessura da malha](../bakers-settings/thickness-map-from-mesh/thickness-map-from-mesh.md)
* [Textura transferida da malha](../bakers-settings/transferred-texture-from/transferred-texture-from-mesh.md)
* [Direção Espacial Global](../bakers-settings/world-space-direction/world-space-direction.md)
* [Normas globais de espaço](../bakers-settings/world-space-normals/world-space-normals.md)

</td>
<td style="border: 0;" valign="top">

### Guias

* [Mensagens de Erro e Aviso](../guides/error-and-warning-mes/error-and-warning-messages.md)
* [Desempenho e otimizações](../guides/performances-and-opt/performances-and-optimizations.md)
* [Triangulação antes da cozedura](../guides/triangulating-before-bak/triangulating-before-baking.md)

</td>
</tr>
</table>

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

### Recursos

* [Cache de geometria](../features/geometry-cache/geometry-cache.md)
* [Rastreamento de raios do GPU](../features/gpu-raytracing/gpu-raytracing.md)
* [Correspondência por nome](../features/matching-by-name/matching-by-name.md)
* [Espaço Tangente](../features/tangent-space/tangent-space.md)

</td>
<td style="border: 0;" valign="top">

### Perguntas comuns

* [Como exportar os mapas baked?](../common-questions/how-export-the-baked-maps/how-to-export-the-baked-maps.md)
* [O pontilhamento é aplicado às texturas feitas bake?](../common-questions/dithering-applied-baked/is-dithering-applied-to-baked-textures.md)
* [Devo ativar “Calcular espaço tangente por fragmento”?](../common-questions/should-enable-compute-tan/should-i-enable-compute-tangent-space-per-fragment.md)
* [A textura feita bake fora do software Substance parece incorreta](../common-questions/texture-baked-outside-sof/texture-baked-outside-of-substance-software-looks-incorrect.md)
* [O que são arquivos Assbin?](../common-questions/what-are-assbin-files/what-are-assbin-files.md)
* [Qual é a profundidade de bits das texturas feitas bake?](../common-questions/what-the-bit-depth-baked/what-is-the-bit-depth-of-baked-textures.md)
* [Qual é a diferença entre o formato normal do OpenGL e do DirectX?](../common-questions/what-the-difference-bet/what-is-the-difference-between-the-opengl-and-directx-normal-format.md)
* [Por que existem trechos estranhos em minhas texturas depois de fazer bake ou exportar?](../common-questions/why-are-there-strange-str/why-are-there-strange-stretches-in-my-textures-after-baking-or-exporting.md)
* [Por que a Correspondência por Nome não está funcionando com a Oclusão de ambiente/Thickness?](../common-questions/why-matching-name-not-wor/why-is-matching-by-name-not-working-with-ambient-occlusion-thickness.md)
* [Por que minha malha está totalmente preta depois de fazer bake?](../common-questions/why-mesh-fully-black-aft/why-is-my-mesh-fully-black-after-baking.md)

</td>
<td style="border: 0;" valign="top">

### Problemas comuns

* [Serrilhado em emendas UV](../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md)
* [A saída do baker está totalmente preta ou vazia](https://helpx.adobe.com/substance-3d/unlisted/documentation/bake/baker-output-is-fully-black-159451835.html)
* [Falha ao fazer bake com Colorir mapa a partir duma malha](../common-issues/baking-failed-with-color/baking-failed-with-color-map-from-mesh.md)
* [Cruz sombreamento preta é visível na superfície da malha](../common-issues/black-shading-cross-are/black-shading-cross-are-visible-on-the-mesh-surface.md)
* [As partes da malha sangram entre si](../common-issues/mesh-parts-bleed-between/mesh-parts-bleed-between-each-other.md)
* [O mapa normal tem gradientes coloridos estranhos](../common-issues/normal-map-has-strange/normal-map-has-strange-colorful-gradients.md)
* [A textura normal parece facetada](../common-issues/normal-texture-looks-fac/normal-texture-looks-faceted.md)
* [As costuras ficam visíveis depois de fazer bake uma textura normal](../common-issues/seams-are-visible-after/seams-are-visible-after-baking-a-normal-texture.md)
* [Costura visível em cada rosto](../common-issues/seam-visible-every-face/seam-visible-on-every-face.md)

</td>
</tr>
</table>
