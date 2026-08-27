---
helpx_url: "https://helpx.adobe.com/br/substance-3d-bake/bakers-settings/curvature-from-mesh.html"
breadcrumb-title: ''
description: Gere texturas de curvatura precisas a partir de malhas de alto polígono usando Rastreamento de raios para a detecção precisa de bordas.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Curvature from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Curvatura da malha
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---


# Curvatura da malha

A Curvatura do baker de malha gera uma textura de curvatura de malhas de alto polígono. É mais lento do que o baker de base [curvatura](../../bakers-settings/curvature/curvature.md), mas produz resultados mais precisos.

**Disponível em:**

* Substance Designer
* Substance Automation Toolkit
* Substance Painter

## Parâmetros

| *Parâmetro* | *Descrição* |
| --- | --- |
| **Raios secundários** | Quantidade de raios emitidos para ler a geometria próxima. Um valor alto produzirá menos ruído, mas levará mais tempo para calcular. O padrão é 32. |
| **Raio de Amostragem** | A distância em que a geometria próxima é considerada para calcular a curvatura na superfície da geometria. Valores altos podem produzir bordas mais fortes, enquanto valores mais baixos podem produzir bordas mais finas, mas faltam informações. |
| **Em Relação À Caixa Delimitadora** | Define se o raio de amostragem é relativo ao tamanho da malha ou se é definido como uma distância baseada em unidades. |
| **Autointerseção** | Correspondência por nome de raios de curvatura. Indica como os padeiros devem corresponder à geometria baixa e alta. Ele pode ser usado para filtrar o processo de cozimento sem a necessidade de mover manualmente (explodir) malhas.Valores possíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Sempre</strong> (padrão): a malha de baixo polígono corresponde a cada malha de alto polígono.</li><li data-preserve-html="true"><strong>Por nome da malha</strong>: filtre as malhas por nome para evitar correspondência com geometria indesejada.</li></ul>Para saber mais sobre a geometria correspondente, consulte: [Correspondência por Nome](../../features/matching-by-name/matching-by-name.md). |
| **Limites de mapeamento automático de tons** | Controla como os valores de curvatura devem ser gravados na textura. Se ativada, o intervalo de valores será normalizado entre 0 e 1 com base nos valores mínimo e máximo encontrados durante o processo de cozimento. Se esta opção estiver desativada, os valores mínimo e máximo serão definidos manualmente.  **Observação:** ao preparar blocos UDIMs/UV, este parâmetro deve ser desabilitado para tornar o mapeamento de tons uniforme e não específico por bloco; caso contrário, isso poderá criar emendas entre cada textura. Para encontrar os valores corretos de mínimo/máximo manualmente, programe primeiro com essa configuração ativada e, em seguida, examine o console/log para ver quais valores foram exportados pelo padeiro. |
| **Mínimo de mapeamento de tons** | Se os **limites do mapeamento automático de tons** estiverem desabilitados, define o valor mínimo para dimensionar o resultado da curvatura para caber na textura. |
| **Máx. de mapeamento de tons** | Se os **limites do mapeamento automático de tons** estiverem desabilitados, define o valor máximo para dimensionar o resultado da curvatura para caber na textura. |
| **Mapa Normal** | Caminho opcional para uma textura normal. Pode ser usado para substituir o cálculo interno do padeiro. |
| **Espaço Mundial** | Se ativada, a textura normal é interpretada como um espaço de mundo normal em vez de um espaço tangente. |
| **Orientação Normal** | Formato da textura Normal, se estiver no Espaço Tangente. Valores possíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>DirectX</strong> (padrão)</li><li data-preserve-html="true"><strong>OpenGL</strong></li></ul> |
