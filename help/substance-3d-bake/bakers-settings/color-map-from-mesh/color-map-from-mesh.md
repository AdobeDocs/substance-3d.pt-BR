---
helpx_url: "https://helpx.adobe.com/br/substance-3d-bake/bakers-settings/color-map-from-mesh.html"
breadcrumb-title: ''
description: Projete propriedades de cores de malhas de alto polígono em texturas para assar policristalinas ou IDs de material para máscaras de seleção.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Color Map from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Mapa de cores da malha
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 4%

---


# Mapa de cores da malha

Este Mapa de cores do mesh baker projeta as propriedades de cores de uma malha de alta definição em uma textura. Ele pode ser usado para assar polypaint ou IDs de material para criar máscaras de seleção.

**Disponível em:**

* Substance Designer
* Substance Automation Toolkit
* Substance Painter

## Parâmetros

| *Parâmetro* | *Descrição* |
| --- | --- |
| **Origem de cores** | Controles a partir dos quais a propriedade da malha de alto polímero na geração de cor deve se basear.Valores possíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Cor do vértice</strong>: lê a cor do vértice e a salva na textura. As cores são interpoladas de vértice para vértice.</li><li data-preserve-html="true"><strong>Cor do material</strong>: lê a cor do material atribuída a uma face de polígono.</li><li data-preserve-html="true"><strong>ID de malha</strong>: atribua uma cor por objeto encontrado.</li><li data-preserve-html="true"><strong>Identificação de Poligrupo/Submalha</strong>: atribua uma cor por subobjeto (também chamado de elemento).</li></ul> |
| **Gerador de cores** | Define como a cor é gerada quando a **Origem da Cor** está definida como **ID da Malha** ou **ID de Poligrupo/Submalha**.Valores possíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Aleatório</strong>: cada objeto ou subobjeto é colorido por uma cor gerada aleatoriamente.</li><li data-preserve-html="true"><strong>Alteração de matiz</strong>: cada objeto ou subobjeto é colorido por uma cor exclusiva com base em um matiz.</li><li data-preserve-html="true"><strong>Escala de cinza</strong>: cada objeto ou subobjeto é colorido por um valor de escala de cinza exclusivo.</li></ul> |
