---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/modo/bump-and-displacement.html"
breadcrumb-title: ''
description: Use mapas de relevo e deslocamento de materiais de Substance no MODO para adicionar detalhes da superfície e profundidade aos seus modelos.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Bump and Displacement
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Relevo e Deslocamento
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '151'
ht-degree: 0%

---


# Relevo e Deslocamento

Trabalhar com o Bump and Deslocamento

Substance pode ter uma saída de height opcional. Você pode usar isso como deslocamento ou relevo. Quando você ativa o height, ele será definido para o efeito de textura de relevo. Para Unity será definido como Unity Bump e Unreal será Unreal Bump. Você pode, então, selecionar o material do item de Substance e definir a Amplitude do relevo de acordo. Se quiser usar o height como deslocamento, você pode alterar o Efeito Camada de material para Sombreamento de superfície > Deslocamento. Em seguida, na Referência do material, defina a Distância do Deslocamento apropriada.

![](../../../assets/bump-1.png)

Neste exemplo, usei o material Irreal, mas alterei o Efeito de camada de relevo irreal para Deslocamento. Em seguida, no Material do item de Substance, defino a Distância do Deslocamento e renderizo o nível de subdivisão adequadamente.

![](../../../assets/dis.png)
