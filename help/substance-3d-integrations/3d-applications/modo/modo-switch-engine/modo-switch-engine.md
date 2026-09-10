---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/modo/modo-switch-engine.html"
breadcrumb-title: ''
description: Alterne entre os mecanismos de Substance da CPU e GPU no MODO para otimizar o desempenho com base no seu hardware.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Modo Switch Engine
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Modo Switch Engine
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---


# Modo Switch Engine

## Substance Engine de switching

Há duas versões do Substance Engine: a CPU e a GPU. O mecanismo da GPU é usado para criar texturas superiores a 2K. O mecanismo da CPU só é capaz de gerar texturas de até 2K. Se precisar de texturas de resolução mais alta, você precisará alternar para o mecanismo da GPU.

Vá para a opção Configurações de Substance no menu Kit de Substance e escolha Alternar Substance Engine. Você precisará reiniciar o MODO para que o mecanismo da GPU seja ativado. Essa configuração atua como uma preferência global. O mecanismo da GPU será ativado sempre que você executar o MODO até que seja trocado manualmente.

>[!NOTE]
>
> **O uso do mecanismo de GPU de Substance exige uma GPU com RAM de vídeo dedicada de 1 GB ou superior. Não há suporte para GPUs integradas.**\
> Nvidia: GeForce 650M de 1 GB ou superior\
> AMD: 6870M ou superior

![](../../../assets/switch.png)
