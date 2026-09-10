---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-questions/why-is-matching-by-name-not-working-with-ambient-occlusion-thickness.html"
breadcrumb-title: ''
description: Entenda por que a Correspondência por Nome não funciona com baker de Oclusão de ambiente e Thickness e encontre alternativas.
helpx_creative_field: ""
helpx_description: "bakers > Common Questions > Why is Matching by Name not working with Ambient OcclusionThickness "
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 'Por que Corresponder por nome não está funcionando com a Espessura de oclusão do ambiente '
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '109'
ht-degree: 0%

---


# Por que a Correspondência por Nome não está funcionando com a Oclusão/Thickness ambiente?

>[!WARNING]
>
> **Pergunta**
> 
> Habilitei a [Correspondência por Nome](../../features/matching-by-name/matching-by-name.md) nos [parâmetros comuns](../../bakers-settings/common-parameters/common-parameters.md) para filtrar e classificar minhas malhas de poli baixas e altas. Por que o padeiro de Oclusão Ambiente a ignora?

>[!NOTE]
>
> **Explicação**
> 
> Os baker Oclusão de ambiente, Thickness e Dobra normal iniciam os raios secundários quando calculam suas texturas. Esses raios têm sua própria configuração de Correspondência por nome.

>[!NOTE]
>
> **Solução : Substance Painter**
> 
> Solução: ative a filtragem de correspondência por nome para os raios secundários nos parâmetros do baker.
