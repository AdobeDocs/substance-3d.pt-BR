---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-questions/should-i-enable-compute-tangent-space-per-fragment.html"
breadcrumb-title: ''
description: Saiba quando ativar o recurso Calcular espaço tangente por fragmento e como ele afeta os resultados da faz bake.
helpx_creative_field: ""
helpx_description: bakers > Common Questions > Should I enable
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Devo ativar
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 1%

---


# Devo ativar “Calcular espaço tangente por fragmento”?

>[!WARNING]
>
> **Pergunta**
> 
> O que significa a configuração “Calcular espaço tangente por fragmento” e o que é seu uso?

>[!NOTE]
>
> **Explicação**
> 
> Quando ativada, essa configuração informa ao baker para executar o cálculo do Espaço tangente no Sombreador de fragmentos (também chamado de Sombreador de pixels) em vez do Sombreador de vértice. Significando que o cálculo será feito por pixel em vez de ser interpolado de vértice para vértice. Essa configuração é usada pelo baker do mapa normal para saber como codificar a textura. Também sabia ler a textura pelos sombreadores.
> 
> Ativar ou desativar esse parâmetro geralmente requer que as texturas sejam reativadas para sincronizá-las com as viewports 3D e os mecanismos de renderização (como o Iray).

>[!NOTE]
>
> **Solução**
> 
> Dependendo do software ou mecanismo de jogo pretendido para renderizar a textura, esta configuração pode ser desativada ou ativada:
> 
> | *Software* | *Calcular espaço tangente por fragmento* |
> | --- | --- |
> | **Mecanismo Irreal 4** | Ativada |
> | **Unidade** | Desativado |
