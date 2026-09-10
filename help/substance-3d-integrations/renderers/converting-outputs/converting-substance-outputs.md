---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/converting-substance-outputs.html"
breadcrumb-title: ''
description: Saiba como converter saídas de material Substance para corresponder a diferentes requisitos e fluxos de trabalho de renderizador.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Converting Substance outputs
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Convertendo saídas de Substance
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 0%

---


# Convertendo saídas de Substance

## Substance Painter

É possível exportar os mapas convertidos do Substance Painter. Uma ampla variedade de predefinições de renderização é compatível, e a simples seleção de uma predefinição converterá os tipos de mapas. (a conversão é baseada no fluxo de trabalho metal/bruto).

![](../../assets/convertpainter.png){width="800px"}

## Plug-in Substance

O plug-in Substance vai gerar saídas e criar materiais automaticamente para fluxos de trabalho específicos. No entanto, com aplicativos DCC e renderizadores de terceiros, pode ser necessário converter manualmente as saídas metálicas/brutas. As integrações a seguir oferecem suporte a fluxos de trabalho de renderização automática e converterão adequadamente qualquer tipo de mapa, se necessário:

* [Substance no Maya](../../3d-applications/maya/using-workflows/using-workflows.md)
* [Substance no 3ds Max](../../3d-applications/3ds-max/3ds-max.md)

## Substance personalizado

Se você estiver criando um Substance personalizado, poderá criar as saídas específicas necessárias para renderizadores como Vray e Corona. Usando o nó de conversão metálico/aspereza (Biblioteca > Utilitários PBR), você pode facilmente converter os mapas de cor de base, aspereza e metálico para o renderizador específico.

![](../../assets/convert-designer.png){width="600px"}
