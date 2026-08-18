---
helpx_url: "https://helpx.adobe.com/br/substance-3d-bake/bakers-settings/ambient-occlusion-from-mesh.html"
breadcrumb-title: ''
description: Crie texturas de oclusão ambiente precisas a partir de malhas de alto polígono usando técnicas de traçado de raio para aprimorar o realismo.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Ambient Occlusion from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Oclusão ambiente da malha
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 2%

---


# Oclusão ambiente da malha

A Oclusão ambiente do padeiro de malha permite assar uma textura de Oclusão ambiente de malhas de alto poli. É mais lento do que a [oclusão ambiente](../../bakers-settings/ambient-occlusion/ambient-occlusion.md) de base, mas produz resultados mais precisos.

**Disponível em:**

* Substance Designer
* Substance Automation Toolkit
* Substance Painter

## Parâmetros

| *Parâmetro* | *Descrição* |
| --- | --- |
| **Raios secundários** | Quantidade de raios de oclusão. Um valor alto produzirá menos ruído, mas levará mais tempo para calcular. O padrão é 64. |
| **Distância mínima do oclusor** | Distância mínima em que os raios de oclusão atingirão a alta geometria poli. O padrão é 0,00001. |
| **Distância Máxima do Ocultador** | Distância máxima em que os raios de oclusão atingirão a alta geometria poli. O padrão é 0.1. |
| **Em relação à caixa delimitadora** | Se ativadas, as unidades são relativas à caixa delimitadora do objeto (1,0 sendo o comprimento diagonal da caixa delimitadora). Se desativada, as unidades usadas para as distâncias de oclusão mínima e máxima são aquelas definidas ao exportar sua malha (metros, centímetros ou quaisquer unidades que sejam a cena exportada). |
| **Ângulo de Propagação** | Ângulo máximo de propagação dos raios de oclusão. O padrão é 180. |
| **Distribuição** | Distribuição angular dos raios de oclusão. Define como os raios são espalhados em um cone do tamanho do ângulo de propagação.Valores possíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Cosseno</strong> (padrão): realista, mas pode levar à linha branca em áreas ocultadas muito finas. Mais adequado para sombreamento e iluminação.</li><li data-preserve-html="true"><strong>Uniforme</strong>: útil para criar degradês lineares. Mais adequado para máscara de camada e outras filtragens.</li></ul> |
| **Ignorar Backface** | Esses parâmetros definem se os raios de oclusão ignoram ocorrências em uma face de fundo (se o polígono alto normal estiver voltado para a direção oposta à do polígono baixo de onde o raio é disparado). Na maioria das vezes, essa configuração deve ser ativada para evitar artefatos. Valores possíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Nunca</strong> (padrão): as faces traseiras nunca são ignoradas</li><li data-preserve-html="true"><strong>Sempre</strong>: as faces traseiras são sempre ignoradas</li><li data-preserve-html="true"><strong>Por nome da malha</strong>: os backfaces são ignorados somente para malhas que correspondem à palavra-chave do sufixo. Consulte os [parâmetros comuns](../../bakers-settings/common-parameters/common-parameters.md).</li></ul> |
| **Auto-oclusão** | Correspondência por nome para raios de oclusão. Indica como os padeiros devem corresponder à geometria baixa e alta. Ele pode ser usado para filtrar o processo de cozimento sem a necessidade de mover manualmente (explodir) malhas.Valores possíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Sempre</strong> (padrão): a malha de baixo polígono corresponde a cada malha de alto polígono.</li><li data-preserve-html="true"><strong>Por nome da malha</strong>: filtre as malhas por nome para evitar correspondência com geometria indesejada.</li></ul>Para saber mais sobre a geometria correspondente, consulte: [Correspondência por Nome](../../features/matching-by-name/matching-by-name.md). |
| **Mapa Normal** | Caminho opcional para uma textura normal. Pode ser usado para substituir o cálculo interno do padeiro. |
| **Espaço Mundial** | Se ativada, a textura normal é interpretada como um espaço de mundo normal em vez de um espaço tangente. |
| **Orientação Normal** | Formato da textura Normal, se estiver no Espaço Tangente. Valores possíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>DirectX</strong> (padrão)</li><li data-preserve-html="true"><strong>OpenGL</strong></li></ul> |
| **Atenuação** | Define como a oclusão é atenuada pela distância do oclusor.Valores possíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Nenhum</strong>: nenhuma atenuação.</li><li data-preserve-html="true"><strong>Linear</strong> (padrão): atenuação progressiva.</li><li data-preserve-html="true"><strong>Suave</strong>: atenuação suave.</li></ul> |
| **Plano terrestre** | Se ativada, simule um plano abaixo da caixa delimitadora da malha no eixo XZ para colidir com raios secundários. Isso simula o sombreamento vindo de uma planta baixa invisível. |
| **Deslocamento do plano horizontal** | Permite afastar o plano da malha para reduzir a intensidade do efeito. O valor é absoluto e não relativo ao tamanho da malha. |
