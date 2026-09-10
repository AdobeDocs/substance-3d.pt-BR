---
helpx_url: "https://helpx.adobe.com/br/substance-3d-bake/common-issues/aliasing-on-uv-seams.html"
breadcrumb-title: ''
description: Corrija os artefatos de suavização que aparecem em emendas UV durante o fça bake ajustando as configurações de suavização de borda e preenchimento.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Aliasing on UV Seams
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Serrilhado em emendas UV
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 0%

---


# Serrilhado em emendas UV

>[!WARNING]
>
> **Problema**
> 
> Manchas ou pontos escuros aparecem na borda das emendas UV depois de fazer bake:
> 
> ![](../../assets/edge-aliasing.png)

>[!NOTE]
>
> **Explicação**
> 
> Quando o Baker grava informações na textura, elas precisam ser convertidas de geometria em pixels. O processamento dessas informações pode introduzir [aliasing](https://en.wikipedia.org/wiki/Aliasing). O alias geralmente ocorre porque a geometria dos UVs não está alinhada com a grade de pixels ou porque os UVs não cobrem pixels suficientes para fornecer resolução suficiente.
> 
> Nas imagens a seguir, a geometria é a sobreposição vermelha. O baker marcará um pixel como cheio se mais da metade de sua superfície for coberta pela geometria (os quadrados brancos são pixels totais e os quadrados pretos são pixels vazios). Na imagem à direita, a grade de pixels tem o dobro da resolução, o que permite uma representação mais precisa da geometria.
> 
> ![](../../assets/aliasing-example-large.png)
> 
> ![](../../assets/aliasing-example-small.png)

>[!NOTE]
>
> **Solução**
> 
> * Aumente a resolução da textura de saída dos Baker.
> * Aumente a configuração de Suavização de borda (observação: pode levar mais tempo para calcular).
> * Alinhe os UVs à grade de pixels no editor de UV do software de modelagem 3D.
> * Dê uma proporção de texel melhor para UVs.
