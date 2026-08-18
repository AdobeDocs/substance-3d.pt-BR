---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/3d-applications/modo/custom-materials.html"
breadcrumb-title: ''
description: Use materiais personalizados do Unreal, Unity e glTF no MODO com o plug-in de Substance para fluxos de trabalho especializados.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Custom Materials
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Materiais personalizados
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 12%

---


# Materiais personalizados

O plug-in Substance suporta os materiais personalizados Unreal, Unity e glTF. Antes de carregar um arquivo sbsar, você pode selecionar o modo de sombreamento que deseja usar.

## Sumário

## Material da Unidade

Ao usar o Material da unidade, o Efeito de camada de material será definido automaticamente. O plug-in Substance colocará o material da unidade diretamente acima do material do item de Substance.

| Saída de Substance | Espaço de cores | Efeito de camada de material |
| --- | --- | --- |
| Cor de base | sRGB | Albedo do Unity |
| Textura reluzente | Linear | Smoothness do Unity |
| Metálico | Linear | Unity Metallic |
| Normal | Linear | Unidade Normal |
| Emissivo | sRGB | Emissão de Unidade **\*definida como sRGB na Imagem Ainda** |
| Altura | Linear | Unity Bump |
| Oclusão de ambiente | Linear | Oclusão de ambiente do Unity |

![](../../../assets/unity-1.png){width="600px"}

## Material irreal

Ao usar o Material irreal, o Efeito de camada de material será definido automaticamente. O plug-in Substance colocará o Material irreal diretamente acima do Material do item de Substance.

| Saída de Substance | Espaço de cores | Efeito de camada de material |
| --- | --- | --- |
| Cor de base | sRGB | Cor de base irreal |
| Rugosidade | Linear | Aspereza irreal |
| Metálico | Linear | Unreal Metallic |
| Normal | Linear | Irreal normal |
| Altura | Linear | Unreal Bump |
| Emissivo | sRGB | Unreal Emissive **\*definido como sRGB na imagem Still** |
| Oclusão de ambiente | Linear | Oclusão ambiente irreal |
| Opacidade | Linear | Opacidade irreal **\*é necessário desmarcar invertido na camada de textura** |

![](https://helpx-prod.scene7.com/is/image/HelpxProd/unreal?$png$&jpegSize=200&wid=1343){width="600px"}

Talvez seja necessário inverter o normal. Você pode fazer isso no menu Ajustes se o Substance tiver um controle para orientação normal. Caso contrário, isso pode ser feito na própria textura. Para obter mais informações, consulte a página “**[Trabalhando com Normais](../../../3d-applications/modo/working-with-normals/working-with-normals.md)**”.

## Material glTF

Ao usar o Material glTF, o Efeito de camada de material será definido automaticamente. O plug-in Substance colocará o material glTF diretamente acima do material do item de Substance.

| Saída de Substance | Espaço de cores | Efeito de camada de material |
| --- | --- | --- |
| Cor de base | sRGB | Cor de base de glTF |
| Rugosidade | Linear | Aspereza de glTF |
| Metálico | Linear | glTF Metálico |
| Normal | Linear | glTF normal |
| Emissivo | sRGB | glTF Emissive **\*definida como sRGB na Imagem Ainda** |
| Oclusão de ambiente | Linear | oclusão de ambiente glTF |

![](../../../assets/gltf.png){width="600px"}

Talvez seja necessário inverter o normal. Você pode fazer isso no menu Ajustes se o Substance tiver um controle para orientação normal. Caso contrário, isso pode ser feito na própria textura. Para obter mais informações, consulte a página “**[Trabalhando com Normais](../../../3d-applications/modo/working-with-normals/working-with-normals.md)**”.
