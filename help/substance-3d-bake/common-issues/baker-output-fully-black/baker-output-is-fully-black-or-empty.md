---
helpx_url: "https://helpx.adobe.com/br/substance-3d-bake/common-issues/baker-output-is-fully-black-or-empty.html"
breadcrumb-title: ''
description: Solucione problemas sobre por que as saídas de panificação estão totalmente pretas ou vazias e saiba como corrigir problemas de malha e UV.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Baker output is fully black or empty
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: A saída Baker é totalmente preta ou vazia
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---


# A saída Baker é totalmente preta ou vazia

>[!WARNING]
>
> **Problema**
> 
> O resultado de um padeiro é uma textura preta ou vazia:
> 
> ![](../../assets/black.png)

>[!NOTE]
>
> **Explicação**
> 
> Uma textura preta significa que o padeiro não conseguiu encontrar as informações necessárias para gerar um resultado. Por exemplo, o processo de cozimento não encontrou a malha de alto-poli para combinar com o baixo-poli, resultando em nada para comparar.

>[!NOTE]
>
> **Solução**
> 
> * Verifique se a malha de alto polietileno necessária para o padeiro foi carregada corretamente (consulte o arquivo de registro/janela para ver se há erros).
> * Verifique se as malhas de baixo ou alto polígono não são muito grandes (mais de um quilômetro) ou muito pequenas (menos de um centímetro).
> * Verifique se o padeiro conseguiu ler/processar a malha (consulte o arquivo de registro/janela para ver se há erros).
> * Verifique se o recurso [Correspondência por Nome](../../features/matching-by-name/matching-by-name.md) não foi configurado corretamente (alguns objetos podem se excluir e nunca se sobrepor).
> * Verifique se os UVs de baixo polígono estão dentro do intervalo 0-1.
