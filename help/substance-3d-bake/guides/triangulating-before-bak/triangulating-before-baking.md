---
helpx_url: "https://helpx.adobe.com/br/substance-3d-bake/guides/triangulating-before-baking.html"
breadcrumb-title: ''
description: Entenda como a triangulação de malha afeta os resultados de cozimento e aprenda as práticas recomendadas para preparar sua geometria.
helpx_creative_field: ""
helpx_description: bakers > Guides > Triangulating before baking
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Triangulação antes da cozedura
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---


# Triangulação antes da cozedura

Malhas 3D podem ser definidas com polígonos com várias bordas de borda por face. Normalmente via quads (4 bordas), às vezes mais (n-gonos).\
Entretanto, o software transforma esses polígonos em triângulos mais tarde, porque é mais fácil gerenciar e executar a computação (especialmente na GPU).

## Como a triangulação pode afetar uma malha?

![](../../assets/triangulation.jpg)

Não há **soluções padrão** para converter Quad/N-Gons em triângulos. Conforme demonstrado na imagem acima, várias opções são válidas.\
É improvável que os padeiros triangulem malhas como um motor de jogo faria porque escolhemos um algoritmo específico em vez de outro.

## Por que triangular antes de assar?

O processo de cozimento lerá a geometria e, em seguida, codifica as informações em texturas.\
Como essas informações são baseadas em UVs e às vezes na topologia de malha, outros softwares podem decodificar as informações incorretamente se eles não leem a geometria da mesma maneira que quando aplicam a textura.

Na imagem abaixo, você pode ver a malha de baixo polígono na parte superior esquerda e a malha de alto polígono na parte superior direita.\
Na parte inferior está o baixo-poli com o mapa normal assado do alto-poli. A malha à esquerda usa uma triangulação idêntica à usada pela Substance Painter ao assar. A malha à direita não exibe e exibe artefatos pretos. Isso ocorre porque há uma incompatibilidade entre como o mapa normal foi preparado e como a malha está triangulada no momento. Isso pode ser corrigido **atualizando a malha e/ou recozinhando**.

![](../../assets/example-triangulation-artifact.jpg)
