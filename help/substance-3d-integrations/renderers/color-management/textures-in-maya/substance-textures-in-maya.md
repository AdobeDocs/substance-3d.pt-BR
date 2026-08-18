---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/color-management/substance-textures-in-maya.html"
breadcrumb-title: ''
description: Defina as configurações de espaço de cor para texturas de Substance no Maya para garantir o gerenciamento de cores e a renderização precisos.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Color Management > Substance textures in Maya
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Texturas de Substance no Maya
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '134'
ht-degree: 0%

---


# Texturas de Substance no Maya

O espaço de cores definido para mapas depende das configurações e regras estabelecidas nas [Configurações de gerenciamento de cores do Maya](https://help.autodesk.com/view/MAYAUL/2020/ENU/?guid=GUID-B260195C-A0FE-4F51-9EA2-099B61B7725A).

O plug-in Substance no Maya está definido como “Ignorar regras de arquivo do espaço de cores” no nó Arquivo. O plug-in cuida da configuração do espaço de cores independentemente do Gerenciamento de cores usando o seguinte:

BaseColor, Difuso, Emissivo, Specular = sRGB\
Normal, height, deslocamento, rugosidade, metálico = RAW

Normalmente, será necessário definir o Espaço de cor como RAW para imagens que representam dados não coloridos. No entanto, essa configuração pode ser afetada pelas regras definidas no Gerenciamento de cores.

![](../../../assets/raw.png)
