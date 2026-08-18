---
helpx_url: "https://helpx.adobe.com/br/substance-3d-bake/common-questions/is-dithering-applied-to-baked-textures.html"
breadcrumb-title: ''
description: Entenda se o pontilhamento é aplicado a texturas cozidas e como ele afeta a qualidade da textura.
helpx_creative_field: ""
helpx_description: "bakers > Common Questions > Is dithering applied to baked textures "
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 'O pontilhamento é aplicado a texturas cozidas '
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '140'
ht-degree: 0%

---


# O pontilhamento é aplicado a texturas assadas?

>[!WARNING]
>
> **Pergunta**
> 
> Os Padeiros oferecem suporte à textura [pontilhamento](https://en.wikipedia.org/wiki/Dither) e, se for o caso, quando ela é aplicada?

>[!NOTE]
>
> **Explicação**
> 
> O pontilhamento é aplicado para evitar bandas em mapas normais de 8 bits, por exemplo:
> 
> ![](../../assets/dither.jpg)

>[!NOTE]
>
> **Solução : Substance Designer**
> 
> O pontilhamento é aplicado automaticamente nas seguintes situações:
> 
> * Quando uma saída Baker é salva em um arquivo de textura de 8 bits
> * Quando uma saída Baker é usada em um nó de bitmap de um gráfico definido como 8 bits.

>[!NOTE]
>
> **Solução : Substance Painter**
> 
> O pontilhamento é uma opção que pode ser ativada ou desativada durante o processo de exportação. Só é aplicado ao exportar para o formato de arquivo de 8 bits para o canal Normal, de Deslocamento e de Height.

>[!NOTE]
>
> **Solução : Kit De Ferramentas De Automação De Substance**
> 
> O pontilhamento não é suportado no momento.
