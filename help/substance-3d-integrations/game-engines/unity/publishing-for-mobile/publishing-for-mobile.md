---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/game-engines/unity/publishing-for-mobile.html"
breadcrumb-title: ''
description: Otimize materiais de Substance para plataformas móveis no Unity ajustando as configurações e as resoluções de textura.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Publishing for Mobile
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Publicação para dispositivos móveis
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 0%

---


# Publicação para dispositivos móveis

>[!NOTE]
>
> **Tamanho da textura em dispositivos móveis**
> 
> A resolução da textura definida no Editor de Unidade será do tamanho publicado no binário do aplicativo. Diminuir a resolução do material da Substance criará texturas com tamanhos de arquivo menores.

## Plataformas

## Apple iOS

1. Verifique se o módulo iOS foi baixado para a versão correspondente do Unity.
1. No Unity, altere o destino da compilação para iOS.
1. Abra as Configurações do reprodutor e altere o campo “Identificação - Identificador do pacote” para algo mais exclusivo. (por exemplo: com.Adobe.iosProject)
1. Construir e executar o jogo.
1. No Xcode, clique no dispositivo iOS e altere a lista suspensa “Assinatura - Equipe” para a ID de equipe do desenvolvedor.
1. No dispositivo iOS, vá para “Configurações - Geral - Gerenciamento de dispositivos” e clique em “Confiar” na ID de equipe de desenvolvedor que é exibida.
1. Execute a compilação do Xcode novamente clicando no botão &#39;Construir e executar esquema atual&#39; (o botão Reproduzir).
1. O jogo deve estar sendo executado no dispositivo iOS.

## SO Android

1. Verifique se o módulo Android foi baixado para a versão correspondente do Unity.
1. No Unity, altere o destino da compilação para Android.
1. Abra as Configurações do reprodutor e altere o campo “Identificação - Identificador do pacote” para algo mais exclusivo. (por exemplo: com.Adobe.androidProject)
1. Construir e executar o jogo.
1. O jogo deve estar em execução no dispositivo Android.
