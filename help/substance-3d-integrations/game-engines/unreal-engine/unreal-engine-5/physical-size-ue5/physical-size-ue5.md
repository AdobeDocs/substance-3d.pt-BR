---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/physical-size-ue5.html"
breadcrumb-title: ''
description: Use as configurações de tamanho físico para dimensionar materiais de Substance com base em dimensões reais no Unreal Engine 5.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Physical Size - UE5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Tamanho físico - UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '163'
ht-degree: 0%

---


# Tamanho físico - UE5

O tamanho físico em materiais de Substance permite que os materiais sejam dimensionados com base em seu tamanho no mundo. Esse valor é definido em Substance Designer e lido em Unreal por meio do sistema de modelos de material.\
O material [Substance\_Triplanar\_Template](../../../../game-engines/unreal-engine/unreal-engine-5/material-template-usage/out-the-box-material-tem/out-of-the-box-material-templates.md) no pai contém um exemplo de como o tamanho físico pode ser usado para dimensionar materiais irreais.



Independentemente dos valores de elevação na malha, os materiais serão ladrilhados com base no tamanho que ocupam no mundo em centímetros. No caso do material rochoso (figura 1), esse valor é de 1,8m (180cm) para cada medição.

![](../../../../assets/rock-material-parameters.png)

Os materiais de Substance que contêm dados de tamanho físico terão seus valores copiados em qualquer nó de parâmetro de vetor de material existente chamado physicalsize.



Como não há valor de deslocamento em materiais no UE5, o modelo de tamanho físico copia o valor como X, Y, X para o mapa triplanar.
