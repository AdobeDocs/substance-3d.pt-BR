---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/thickness-map-from-mesh.html"
breadcrumb-title: ''
description: Gere mapas de espessura lançando raios para dentro das superfícies da malha para uso em sombreadores e mascaramento SSS.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Thickness Map from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Mapa de espessura da malha
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 5%

---


# Mapa de espessura da malha

O mapa de Espessura da malha é muito semelhante ao baker de oclusão de ambiente, mas ele lança raios da superfície da malha para o interior. Essa textura pode ser usada em um sombreador SSS (Sub Surface Scattering) ou em texturas de mascaramento.

As propriedades da textura são definidas como:

* Os valores de preto representam as partes finas do modelo.
* Os valores de branco representam as partes grossas do modelo.

**Disponível em:**

* Substance Painter
* Substance Designer
* Substance Automation Toolkit

## Parâmetros

| *Parâmetro* | *Descrição* |
| --- | --- |
| **Raios secundários** | Quantidade de raios de oclusão. Um valor alto produzirá menos ruído, mas levará mais tempo para calcular. O padrão é 64. |
| **Distância mínima do oclusor** | Distância mínima em que os raios de oclusão atingirão a alta geometria poli. O padrão é 0,00001. |
| **Distância Máxima do Ocultador** | Distância máxima em que os raios de oclusão atingirão a alta geometria poli. O padrão é 0.1. |
| **Em relação à caixa delimitadora** | Se ativadas, as unidades são relativas à caixa delimitadora do objeto (1,0 sendo o comprimento diagonal da caixa delimitadora). Se desativada, as unidades usadas para as distâncias de oclusão mínima e máxima são aquelas definidas ao exportar sua malha (metros, centímetros ou quaisquer unidades que sejam a cena exportada). |
| **Ângulo de Propagação** | Ângulo máximo de propagação dos raios de oclusão. O padrão é 180. |
| **Distribuição** | Distribuição angular dos raios de oclusão.Valores possíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Cosseno</strong> (padrão)</li><li data-preserve-html="true"><strong>Uniforme</strong></li></ul> |
| **Ignorar Backface** | Se ativados, os raios de oclusão ignoram as ocorrências em uma face traseira (se o polígono alto normal estiver voltado para a direção oposta à do polígono baixo de onde o raio é disparado). Na maioria das vezes, essa configuração deve ser ativada para evitar artefatos. |
| **Auto-oclusão** | Correspondência por nome para raios de oclusão. Indica como os baker devem corresponder à geometria baixa e alta. Ele pode ser usado para filtrar o processo de fça bake sem a necessidade de separar manualmente (explodir) malhas.Valores possíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Sempre</strong> (padrão): a malha de baixo polígono corresponde a cada malha de alto polígono.</li><li data-preserve-html="true"><strong>Por nome da malha</strong>: filtre as malhas por nome para evitar correspondência com geometria indesejada.</li></ul>Para saber mais sobre a geometria correspondente, consulte: [Correspondência por Nome](../../features/matching-by-name/matching-by-name.md). |
| **Normalização Automática** | Define se os valores de saída devem ser dimensionados para se ajustarem a um intervalo de 0-1 (o ponto mais claro é definido como branco puro e o ponto mais escuro é definido como preto puro). |
