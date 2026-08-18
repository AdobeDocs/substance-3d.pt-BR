---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/renderers/color-management.html"
breadcrumb-title: ''
description: Entenda o gerenciamento de cores e a correção de gama ao usar materiais de Substance com renderizadores diferentes.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Color Management
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Gerenciamento de Cores
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 2%

---


# Gerenciamento de Cores

Adotaremos uma abordagem simplista ao afirmar que a renderização de espaço linear fornece a matemática correta para cálculos de iluminação. Cria um ambiente que permite que as interações de luz sejam representadas de forma credível no mundo real. Para uma discussão sobre renderização de espaço linear, devemos introduzir o conceito de correção gama. Ao codificar imagens para exibição e armazenamento, a correção de gama é o processo de otimização que reduz a largura de banda e a alocação de bits. Esse processo aproveita a percepção de brilho do olho humano, que segue aproximadamente a raiz cúbica de luminância.

>[!NOTE]
>
> A renderização do espaço linear é um assunto altamente complexo. Para obter mais informações, examine o [VOLUME UM DO GUIA PBR](https://academy.substance3d.com/courses/the-pbr-guide-part-1) no [Instituto Substance](https://academy.substance3d.com/).

## Gerenciamento de Cores

A finalidade deste documento é detalhar o processo de trabalho com texturas exportadas de **Substance Painter** e **Substance Designer** no [software 3D](https://www.adobe.com/br/products/substance3d/3d-augmented-reality.html) e renderizadores.

A maneira correta de interpretar uma imagem usada como entrada para um canal de material depende de como a imagem é usada na cena. O espaço da cor, a codificação e se os valores de cor são proporcionais à **luminância com referência em cena** ou à **luminância com referência em exibição** também desempenham um papel importante.

* As imagens usadas para representar **dados sem cor** não devem ser transformadas. Geralmente, são mapas de **normais**, **aspereza**, **metálicos**, **deslocamentos** e **ambientes** **oclusões**.
* As imagens que representam as cores que vemos podem ter vários cenários. Por exemplo, imagens que já são **lineares para a cena** normalmente não precisam ser convertidas, como imagens de **intervalo dinâmico alto** armazenadas em formatos como **OpenEXR** e **HDR**.
* A gama das imagens criadas para exibição (**com referência em exibição**) precisa ser removida. Isso inclui a maioria dos formatos, como **PNG**, **JPEG** e **BMP**. Estas imagens são **básicas**, **coloridas**, **difusas**, **speculares** e **emissivas**.

Embora esta seja uma simplificação excessiva, pode ser útil pensar no processo da seguinte forma:

* “com referência em cena (por exemplo, linear)” : Não aplicar uma conversão
* “com referência em exibição (por exemplo, sRGB)” : aplicar a transformação inversa para “linearizar” a imagem para o cálculo adequado

>[!NOTE]
>
> A função de decodificação sRGB (EOTF) que converte de espaço gama para espaço linear é usada em Substance Painter e Substance Designer e é definida pelo padrão IEC 61966-2-1:1999

O Substance Designer pode ser configurado para usar o [OpenColorIO](https://opencolorio.org/) para o Gerenciamento de Cores. Isso permite que você tenha transformações de cores *consistentes* e exibição de imagens em vários aplicativos. Nesse modo, o Substance Designer funcionará internamente com **RGB linear** cores. Como a profundidade de bits de 8 não é normalmente suficiente para representar cores lineares, é recomendável usar a profundidade de *pelo menos* **16 bits** para texturas de cores no [gráfico](https://docs.substance3d.com/display/SDDOC/Graph+View).

![](https://helpx-prod.scene7.com/is/image/HelpxProd/sd-cm?$png$&jpegSize=200&wid=686)

Quando introduzimos o [ACES](https://www.oscars.org/science-technology/sci-tech-projects/aces), agora temos dois espaços de cores diferentes, o sRGB linear (a versão sem gama do sRGB) e o [ACEScg](https://acescolorspace.com/), que é um espaço de cores de gama ampla (”referenciado à cena” ou linear) mais adequado para a renderização CG.

*Gráfico de gamut -<https://acescolorspace.com/>*

O Substance Designer também oferece suporte ao **Adobe Color Engine (ACE)**. Com o **ACE**, você pode escolher seu espaço de cores de trabalho entre **sRGB**, **sRGB linear** e **ACEScg**. Ao usar o **sRGB**, o **ACE** é basicamente o mesmo que o modo herdado. Ao usar um espaço de cores linear, o **ACE** é mais ou menos como o [OpenColorIO](https://opencolorio.org/index.html).

## Plug-ins do Substance

Ao usar materiais de Substance por meio do plug-in de integração de Substance, as saídas são sinalizadas para linear/gama automaticamente por meio da integração e do gerenciamento de cores do aplicativo host. No entanto, é importante entender o processo: quando mapas de Substance são usados como bitmaps exportados em vez de materiais de Substance, pode ser necessário sinalizar manualmente as texturas como **codificadas em gama** ou **brutas** dependendo do renderizador que você está usando. Normalmente, os arquivos .png, .jpg, .tga ou .tif de 8 ou 16 bits são codificados em gama, enquanto os arquivos **sRGB OETF** e .exr são lineares.

## Aplicativos 3D

### Trabalhar com texturas

* [Texturas de Substance no Maya](../../renderers/color-management/textures-in-maya/substance-textures-in-maya.md)
* [texturas de Substance em 3ds Max](../../renderers/color-management/textures-in-3ds-max/substance-textures-in-3ds-max.md)
