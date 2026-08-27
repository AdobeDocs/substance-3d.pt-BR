---
helpx_url: "https://helpx.adobe.com/br/substance-3d-bake/bakers-settings/ambient-occlusion.html"
breadcrumb-title: ''
description: Aprenda a usar o padeiro de Oclusão ambiente para gerar texturas de sombra ambiente usando algoritmos acelerados por GPU rápidos.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Ambient Occlusion
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Oclusão de ambiente
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 4%

---


# Oclusão de ambiente

O padeiro de Oclusão ambiente permite assar uma textura de sombra ambiente. Esse padeiro usa um algoritmo rápido executado na GPU.

**Disponível em:**

* Substance Designer
* Substance Automation Toolkit

>[!WARNING]
>
> * Esse padeiro pode não ser compatível com GPUs antigas.
> * Assumir a alta resolução em GPUs low-end/móveis pode causar uma falha.

## Parâmetros

| *Nome* | *Descrição* |
| --- | --- |
| **Mapa Normal** | Insira o arquivo de mapa normal que pode ser usado para fornecer detalhes adicionais de geometria na superfície da malha a serem considerados durante o cálculo do padeiro. Esse parâmetro é opcional. |
| **Espaço Mundial** | Se habilitado, especifique que o mapa normal de entrada está no Espaço Mundial (em vez do Espaço Tangente). Se nenhum mapa de entrada normal for fornecido, esses parâmetros serão ignorados/desabilitados. |
| **Inverter normal** | Calcula o mapa de oclusão ambiente com normais invertidos (pode ser usado para gerar um mapa de thickness). |
| **Usar partes de malha não selecionadas** | Use partes de malha não selecionadas da malha para assar o mapa de oclusão ambiente. |
| Qualidade **1** | Escolha a qualidade do mapa de Oclusão ambiente. Uma qualidade mais alta é mais lenta de calcular.Valores disponíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Baixo</strong> (3 passos)</li><li data-preserve-html="true"><strong>Médio</strong> (padrão, 5 passos)</li><li data-preserve-html="true"><strong>Alto</strong> (10 passos)</li><li data-preserve-html="true"><strong>Muito Alta</strong> (16 passadas)</li></ul> |
| **Polarização de Precisão** | Precisão da oclusão de ambiente. Um valor mais baixo fornecerá uma precisão mais alta, mas poderá produzir artefatos maiores. |
| **Desvanecer à Distância** | Dispersão da oclusão do ambiente. |
