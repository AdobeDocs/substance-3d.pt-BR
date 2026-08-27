---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/bent-normals-from-mesh.html"
breadcrumb-title: ''
description: Texturas de dobras normais de computação que descrevem a direção média da iluminação ambiente a partir de malhas de alto polígono.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Bent Normals from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Normais tortos da malha
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 3%

---


# Normais tortos da malha

As Dobras normais do baker de malha calculam uma textura que descreve a direção média da iluminação ambiente. Este baker é derivado da [Oclusão de ambiente do baker Mesh](../../bakers-settings/ambient-occlusion-from/ambient-occlusion-from-mesh.md).

**Disponível em:**

* Painter
* Designer
* Kit de ferramentas de automação

## Parâmetros

| *Parâmetro* | *Descrição* |
| --- | --- |
| **Raios secundários** | Quantidade de raios de oclusão. Um valor alto produzirá menos ruído, mas será mais longo para calcular. |
| **Distância mínima do oclusor** | Distância mínima em que os raios de oclusão atingirão a alta geometria do polígono&#x200B;**.** |
| **Distância Máxima do Ocultador** | Distância máxima em que os raios de oclusão atingirão a alta geometria poli. |
| **Em relação à caixa delimitadora** | Se ativado, os cálculos de distância de raio são baseados no espaço normalizado (0 a 1) da malha de baixo-polímero. Se desativado, o cálculo da distância de raio é baseado em unidades especificadas na malha de baixo polímero quando ele foi exportado (metros, centímetros etc.). |
| **Ângulo de Propagação** | Ângulo máximo de propagação dos raios de oclusão. O padrão é 180. |
| **Distribuição** | Distribuição angular dos raios de oclusão.Valores possíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Cosseno</strong> (padrão)</li><li data-preserve-html="true"><strong>Uniforme</strong></li></ul> |
| **Ignorar Backface** | Se ativados, os raios de oclusão ignoram as ocorrências em uma face traseira (se o polígono alto normal estiver voltado para a direção oposta à do polígono baixo de onde o raio é disparado). Na maioria das vezes, essa configuração deve ser ativada para evitar artefatos. |
| **Auto-oclusão** | Correspondência por nome para raios de oclusão. Indica como os padeiros devem corresponder à geometria baixa e alta. Ele pode ser usado para filtrar o processo de cozimento sem a necessidade de mover manualmente (explodir) malhas.Valores possíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Sempre</strong> (padrão): a malha de baixo polígono corresponde a cada malha de alto polígono.</li><li data-preserve-html="true"><strong>Por nome da malha</strong>: filtre as malhas por nome para evitar correspondência com geometria indesejada.</li></ul>Para saber mais sobre a geometria correspondente, consulte: [Correspondência por Nome](../../features/matching-by-name/matching-by-name.md). |
| **Tipo de Mapa** | Define o tipo da textura de saída.Valores possíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Espaço mundial</strong></li><li data-preserve-html="true"><strong>Espaço tangente</strong> (padrão)</li></ul> |
| **Orientação Normal** | Controla o formato normal da textura de saída se **Mat Type** estiver definido como Espaço tangente.Valores possíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>OpenGL</strong> <strong> <br/></strong></li><li data-preserve-html="true"><strong>DirectX</strong> (padrão)<strong> <br/></strong></li></ul> |
