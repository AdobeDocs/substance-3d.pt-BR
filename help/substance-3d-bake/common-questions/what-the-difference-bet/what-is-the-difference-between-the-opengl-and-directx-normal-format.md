---
helpx_url: "https://helpx.adobe.com/br/substance-3d-bake/common-questions/what-is-the-difference-between-the-opengl-and-directx-normal-format.html"
breadcrumb-title: ''
description: Conheça as diferenças entre os formatos de mapa normais OpenGL e de DirectX e quando usar cada um deles.
helpx_creative_field: ""
helpx_description: "bakers > Common Questions > What is the difference between the OpenGL and DirectX normal format "
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 'Qual é a diferença entre o formato normal do OpenGL e do DirectX '
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 0%

---


# Qual é a diferença entre o formato normal do OpenGL e do DirectX?

>[!WARNING]
>
> **Pergunta**
> 
> Qual é a diferença entre o formato normal do OpenGL e do DirectX?

>[!NOTE]
>
> **Explicação**
> 
> OpenGL e DirectX são duas APIs gráficas (conjuntos de funções) que os programadores usam em seu aplicativo para dialogar com a GPU (Unidade de processamento gráfico). Em termos de mapas normais, a diferença resulta em como o canal verde de uma textura de RGB deve ser interpretado. O OpenGL espera que o primeiro pixel esteja na parte inferior, enquanto o DirectX espera que ele esteja na parte superior. É por isso que, em várias discussões técnicas, é recomendado tentar inverter o canal verde de um mapa normal para ver se ele se comporta melhor à medida que inverte os valores de pixel (o primeiro se torna o último). O OpenGL pode ser referido como **Y+** (de baixo para cima), enquanto o DirectX é referido como **Y-** (de cima para baixo).
> 
> Para saber qual formato usar, consulte o aplicativo de destino no qual as texturas serão usadas.
