---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/curvature.html"
breadcrumb-title: ''
description: Extraia informações de curvatura da malha para criar texturas que destacam cavidades e bordas da geometria.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Curvature
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Curvatura
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 2%

---


# Curvatura

O padeiro de curvatura permite extrair uma textura de curvatura. Essa textura contém cavidades e informações de bordas relacionadas à geometria.

As propriedades da textura são definidas como:

* Os valores de preto representam áreas côncavas.
* Os valores de branco representam áreas convexas.
* Os valores de cinza representam áreas neutras (principalmente planas).

**Disponível em:**

* Substance Designer
* Substance Automation Toolkit
* Substance Painter

## Parâmetros

| *Parâmetro* | *Descrição* |
| --- | --- |
| **Algoritmo** | Define como as informações de curvatura serão computadas na malha. |
| **Detalhes** | Controla a intensidade das informações na curvatura. Um valor alto pode produzir mais detalhes, mas menos sutileza. |
| **Habilitar Transmissões** | Se ativado, o padeiro tentará reduzir as emendas entre as Ilhas UV copiando os texels nas bordas de um lado para o outro. |
| **Faixas** **Intensidade** | Se **Habilitar costuras** estiver habilitado, este parâmetro controlará a intensidade da correção de costuras. |
