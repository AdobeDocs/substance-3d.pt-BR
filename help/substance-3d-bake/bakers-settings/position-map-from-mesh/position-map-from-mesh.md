---
helpx_url: "https://helpx.adobe.com/br/substance-3d-bake/bakers-settings/position-map-from-mesh.html"
breadcrumb-title: ''
description: Calcule mapas de posição precisos a partir de malhas de alto polígono para capturar informações precisas de localização da geometria.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Position map from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Mapa de posição da malha
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---


# Mapa de posição da malha

O mapa de posição do baker de malha calcula o local da geometria de malha de alto polígono e salva em uma textura. É semelhante ao baker da posição base, mas pode produzir resultados mais precisos.

**Disponível em:**

* Substance Designer
* Substance Automation Toolkit

## Parâmetros

| *Parâmetro* | *Descrição* |
| --- | --- |
| **Modo** | Controla quais informações serão computadas na textura de posição.Valores possíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Todos os eixos:</strong> Faz bake a posição dos eixos X, Y e Z nos canais de RGB da textura de saída.</li><li data-preserve-html="true"><strong>Um eixo:</strong> Faz bake um único eixo na textura de saída como uma imagem em tons de cinza.</li></ul> |
| **Eixo** | Define qual eixo deverá ser calculado se o parâmetro **Modo** estiver definido como **Um eixo**. |
| **Tipo de Normalização** | Define como dimensionar os valores de posição por eixo.Valores possíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Caixa:</strong> normalize cada eixo de acordo com o volume da malha (comprimento da caixa delimitadora).</li><li data-preserve-html="true"><strong>BSphere:</strong> normalize todos os eixos de acordo com o raio do volume da malha (esfera delimitadora).</li></ul> |
| **Escala de Normalização** | Define como dimensionar os valores de posição com base na malha.Valores possíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Por material</strong>: os valores são dimensionados entre 0 e 1 para cada material (conjunto de texturas).</li><li data-preserve-html="true"><strong>Cena Completa</strong> (padrão): os valores são dimensionados para levar a malha inteira em consideração. Isso permite valores de posição contínuos em objetos e materiais (conjuntos de texturas).</li></ul> |
