---
helpx_url: "https://helpx.adobe.com/br/substance-3d-bake/common-issues/baking-failed-with-color-map-from-mesh.html"
breadcrumb-title: ''
description: Resolva falhas de fça bake de Colorir mapa a partir duma malha verificando as propriedades de cor de malha e o mapeamento UV.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Baking failed with Color Map from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Falha na cozedura com o Mapa de cores da malha
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---


# Falha na cozedura com o Mapa de cores da malha

>[!WARNING]
>
> **Problema**
> 
> Possível mensagem de erro:
> 
> &#x200B;> > > 
> 
> [ Fazendo bake ] Falha ao Fazer bake (Colorir mapa a partir duma malha)\
> Não foi possível localizar as cores do vértice

>[!NOTE]
>
> **Explicação**
> 
> As configurações padrão para o [Colorir mapa a partir duma malha](../../bakers-settings/color-map-from-mesh/color-map-from-mesh.md) é fazer bake as cores de vértice de malha de alto polígono em uma textura com base nos UVs de malha. No entanto, muitas vezes é o caso em que a malha de alto-poli não tem nenhuma informação de cores de vértice. Portanto, o baker não pode gravar informações que não existem.

>[!NOTE]
>
> **Solução**
> 
> Soluções diferentes estão disponíveis para evitar esta mensagem de erro:
> 
> * Usar uma malha de alto polígono com cores de vértice
> * Defina o baker do Colorir mapa a partir duma malha com configurações diferentes
> * Não use o baker Colorir mapa a partir duma malha se não precisar dele
