---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/rendering-color-space.html"
breadcrumb-title: ''
description: Defina as configurações do espaço de cores do Unity para garantir a renderização adequada de materiais de Substance com sombreadores baseados fisicamente.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Rendering Color Space
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Espaço de cor de renderização
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '102'
ht-degree: 0%

---


# Espaço de cor de renderização

As texturas Substance são projetadas para serem usadas com um sombreador baseado em Física. Para obter os melhores resultados, você deve definir o espaço da cor como linear nas Configurações do Unity Player.

1. Acesse Editar > Configurações do projeto > Player.
1. Na seção Renderização, altere o Espaço de cor para Linear. (O padrão da unidade é Espaço gama, que está incorreto e resultará na aparência incorreta da cor da textura).

   >[!NOTE]
   >
   > **Informações**
   > 
   > As opções de sRGB no textura são desativadas se a Configuração do espaço da cor no Unity for definida como Gama

   ![](../../../assets/rendering-4.png){width="600px"}
