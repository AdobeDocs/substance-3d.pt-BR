---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-issues/normal-texture-looks-faceted.html"
breadcrumb-title: ''
description: Corrija a aparência facetada em texturas normais suavizando os normais de malha e ajustando as configurações de grupo de suavização.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Normal texture looks faceted
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: A textura normal parece facetada
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---


# A textura normal parece facetada

>[!WARNING]
>
> **Problema**
> 
> A textura Normal parece facetada ou cada face da malha é visível nela após assá-la.
> 
> ![](../../assets/normal-faceted.jpg)

>[!NOTE]
>
> **Explicação**
> 
> A principal razão pela qual assar um normal produziria este resultado é porque os normais de malha poli baixa não estão definidos corretamente. Cada borda de cada faces é uma borda dura, fazendo a projeção de raio durante a correspondência com a malha de alto-poli ignorar informações vizinhas e cria costuras ou informações inconscientes. Embora o resultado possa parecer normal na malha, isso pode levar a problemas de sombreamento mais tarde e deve ser resolvido.

>[!NOTE]
>
> **Solução**
> 
> A solução principal é retrabalhar o vértice normal ou a malha poli baixa, a nomeação exata do processo depende do software de modelagem 3D:
> 
> * Use os **normais médios** no Maya, Houdini.
> * Use **um grupo de suavização** no 3DS Max.
> * Use **sombra suave** no Blender.
> * As malhas exportadas do zBrush sempre serão facetadas e deverão ser limpas em outro software.
> 
> Observe que isso pode não ser suficiente: certifique-se de que as configurações também salvem/gerem as informações normais de vértice ou de sombreamento ao exportar uma malha.
