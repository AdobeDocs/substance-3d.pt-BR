---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/live-link-in-ue4.html"
breadcrumb-title: ''
description: Use o Live Link no Unreal Engine 4 para sincronizar materiais de Substance entre o Painter e o UE4 em tempo real.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Live Link in UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Live Link na UE4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 0%

---


# Live Link na UE4

>[!WARNING]
>
> O Live Link no Unreal Engine não é mais compatível. Os usuários com uma versão mais antiga do plug-in em que o Live Link é usado ainda poderão usar o recurso.

>[!WARNING]
>
> O Live Link não funciona com malhas UE4 BSP. O ativo enviado precisa ser um arquivo de modelo importado para o projeto UE4

## Estabelecendo link para o Substance Painter

1. Abrir Substance Painter
1. Clique com o botão direito no ativo que deseja enviar para o Painter no Navegador de conteúdo e escolha “Enviar para o Painter”.

   ![](../../../../assets/link1-22.png){width="400px"}
1. A malha aparecerá em Substance Painter e você poderá iniciar a texturização. À medida que você trabalha, as texturas são enviadas para UE4 e aplicadas aos materiais. O ponto verde no ícone UE4 na barra de ferramentas indica que o link está ativo e enviando texturas.

   ![](../../../../assets/icon-12.png)

   1. Você pode pausar o fluxo de dados nas opções de configuração do plug-in. Acesse Plugins>dcc-live-link e escolha Configurar. Desative a opção Habilitar Streaming para pausar o envio de dados para o UE4.

      ![](https://helpx-prod.scene7.com/is/image/HelpxProd/config-6?$png$&jpegSize=100&wid=393)
1. As texturas do Painter serão exibidas no Navegador de conteúdo e aplicadas ao material no UE4.

   ![](../../../../assets/link3-11.png){width="500px"}
1. Um projeto Substance Painter (.spp) será criado na pasta do projeto UE4 em uma pasta rotulada “.sp”

   ![](../../../../assets/link4-5.png)

## Restabelecer um link para o Substance Painter

Você pode continuar de onde parou após fechar o Painter ou o Unity.

1. Abra o projeto .spp no Substance Painter localizado na pasta Unity project>assets>.sp.
1. Clique com o botão direito do mouse na malha no Navegador de conteúdo e escolha “Enviar para o Painter” para restabelecer o link.

   ![](../../../../assets/link5-3.png){width="600px"}
