---
helpx_url: "https://helpx.adobe.com/br/substance-3d-bake/bakers-settings/world-space-direction.html"
breadcrumb-title: ''
description: Calcule as direções vetoriais no espaço mundial e salve-as em texturas para efeitos direcionais e mascaramento.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > World Space Direction
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Direção Espacial Global
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 4%

---


# Direção Espacial Global

O baker de direção do espaço mundial permite calcular uma direção vetorial no espaço mundial em uma textura.

**Disponível em:**

* Substance Designer
* Substance Automation Toolkit

## Parâmetros

| *Parâmetro* | *Descrição* |
| --- | --- |
| **Direção de entrada** | Define a partir de qual entrada a direção é calculada.Valores possíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Da Textura</strong>: a direção do vetor é definida por uma textura de entrada.</li><li data-preserve-html="true"><strong>De Vetor Uniforme</strong> (padrão): a direção do vetor é definida com os controles deslizantes X, Y, Z.</li></ul> |
| **Orientação Normal** | Define o formato normal da textura de saída. Isso inverte o canal verde dependendo do formato.Valores possíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>OpenGL</strong></li><li data-preserve-html="true"><strong>DirectX</strong> (padrão)</li></ul> |
| **X Y Z** | Controles deslizantes para definir os 3 componentes do vetor de direção, se a **Direção de Entrada** estiver definida como **De Vetor Uniforme**. |
| **Arquivo de Direção** | Caminho para o arquivo de textura de entrada para definir o vetor de direção, se a **Direção de Entrada** estiver definida como **Da Textura**. |
