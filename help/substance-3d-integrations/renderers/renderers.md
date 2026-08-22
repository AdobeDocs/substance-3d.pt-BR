---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/renderers.html"
breadcrumb-title: ''
description: Use materiais de Substance com renderizadores principais, como Arnold, V-Ray, Redshift e outros, em seu fluxo de trabalho 3D.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Renderizadores
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 1%

---


# Renderizadores

Os materiais de Substance fornecidos em [Substance Source](https://source.substance3d.com/) contêm saídas para sombreadores baseados em Física e oferecem suporte para os fluxos de trabalho [Metálico/Aspereza (fluxo de trabalho padrão) e Specular/Textura reluzente](https://academy.substance3d.com/courses/pbrguides). É importante entender o fluxo de trabalho ao qual o material do renderizador oferece suporte. Dependendo do renderizador, talvez você consiga usar saídas de material de Substance diretamente ou talvez precise converter as texturas de saída. Os materiais de Substance personalizados ou materiais baixados do Substance share podem não conter as saídas apropriadas necessárias para um determinado renderizador.

![](../assets/outputs.png){width="200px"}

Por exemplo, com Arnold ou Vray Next, é possível usar saídas metálicas/de aspereza diretamente. No entanto, com a pxrSurface do Renderman, as saídas de basecolor/metálicas precisam ser convertidas para a cor da face difusa e do specular. Um plug-in de integração de Substance tratará essas conversões automaticamente se o renderizador for compatível.

Com o Substance Painter, você pode escolher um [Modelo de saída](https://experienceleague.adobe.com/pt-br/docs/substance-3d-painter/using/getting-started/export/export-window/export-window) que criará os tipos de mapa apropriados necessários para um determinado renderizador. Se o seu renderizador não for suportado por padrão, você também pode criar Modelos de saída personalizados.

**Modelo de saída de Substance Painter**

![](../assets/output-template.png){width="500px"}

## Guias do renderizador

* [Convertendo saídas de Substance](../renderers/converting-outputs/converting-substance-outputs.md)
* [Gerenciamento de Cores](../renderers/color-management/color-management.md)
* [Arnold](../renderers/arnold/arnold.md)
* [Variar](../renderers/vray/vray.md)
* [Renderman](../renderers/renderman/renderman.md)
* [Redshift](../renderers/redshift/redshift.md)
* [Maxwell](../renderers/maxwell/maxwell.md)
* [Corona](../renderers/corona/corona.md)
* [Octano](../renderers/octane/octane.md)
* [Keyshot](../renderers/keyshot/keyshot.md)
* [Thea](../renderers/thea/thea.md)
* [Maverick](../renderers/maverick/maverick.md)
* [Toolbag](../renderers/toolbag/toolbag.md)
* [Ciclos e véspera](../renderers/cycles-and-eevee/cycles-and-eevee.md)
