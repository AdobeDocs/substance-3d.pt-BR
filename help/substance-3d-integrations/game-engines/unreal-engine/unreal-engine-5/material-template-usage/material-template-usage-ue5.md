---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/material-template-usage-ue5.html"
breadcrumb-title: ''
description: Crie e use modelos de material no Unreal Engine 5 para definir como os nós de saída de Substance se conectam às entradas de material.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Material Template Usage - UE5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Uso do Modelo de Material - UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 0%

---


# Uso do Modelo de Material - UE5

Os modelos de material permitem que o usuário crie um material de base para que as substâncias sejam usadas como um modelo para conectar seus nós de saída às entradas no material.\
Saídas que compartilham o mesmo nome e tipo que uma entrada de material serão usadas automaticamente. Este exemplo de material pai tem um nó de amostra de textura “baseColor” que será preenchido se o Substance tiver uma saída de textura também chamada “baseColor”.\
![](../../../../assets/parent-material-sample.png)

As saídas de Substance suportam a atualização de texturas, valores float simples ou int escalar e valores vetoriais (2-4). Para usar saídas float ou int no tempo de execução, você deve obter o dynamicMaterialInstance do gráfico, pois o constantMaterialInstances (qualquer material gerado no editor) não pode alterar valores escalares no tempo de execução.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/scalar-value?$png$&jpegSize=100&wid=245)

A ocorrência do gráfico do substance tentará preencher todos os valores de saída relevantes no momento da criação.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/screen-shot-2022-04-01-at-4-38-31-pm?$png$&jpegSize=200&wid=1076)
