---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/optimization-guidelines.html"
breadcrumb-title: ''
description: Siga as diretrizes de otimização para equilibrar a complexidade do material de Substance com o desempenho de renderização no Unity.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Optimization Guidelines
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Diretrizes de otimização
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---


# Diretrizes de otimização

Quanto mais complexos forem seus materiais Substance, mais poder de processamento será necessário para renderizá-los. Os materiais do Substance devem, portanto, **encontrar um equilíbrio entre a complexidade e a velocidade de renderização**. Isso é *especialmente* importante se for usado em aplicativos gráficos em tempo real, como jogos.

Ao criar seus próprios materiais de Substance personalizados, verifique as diretrizes de otimização a seguir.

[Diretrizes de otimização de Substance Designer](https://docs.substance3d.com/display/SDDOC/Performance+Optimization+Guidelines)

Uma advertência importante a ser observada são os nós que têm uma resolução absoluta de 4K ou superior.

>[!WARNING]
>
> **Preste muita atenção à resolução e às configurações de resolução relativas ao pai!**\
> Valores altos afetarão seriamente o desempenho, portanto, considere como o material é susceptível de ser usado e se você pode reduzir os tamanhos dos dados envolvidos.
>   
> O mecanismo da CPU Substance pode computar em 4K, mas é muito lento e pode causar um travamento na integração ou possivelmente um travamento.

No exemplo a seguir, o tamanho de saída de um nó [Tile Sampler](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/substance-graphs/nodes-reference-for-substance-graphs/node-library/texture-generators/patterns/tile-sampler) está definido como [Absoluto](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/substance-graphs/output-size) 4096. Ele faz com que vários nós downstream sejam computados em 4K antes de serem reduzidos para a resolução de saída final de 2048.

![](../../../assets/absolute.png){width="1000px"}
