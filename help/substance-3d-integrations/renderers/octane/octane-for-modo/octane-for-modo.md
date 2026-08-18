---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/renderers/octane/octane-for-modo.html"
breadcrumb-title: ''
description: Use materiais de Substance com renderizador de octano no MODO por meio de materiais Live DB e configurações de saída adequadas.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Octane > Octane for MODO
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Octano para MODO
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---


# Octano para MODO

## Substance no plug-in MODO

As saídas de Substance funcionam de forma nativa com octano. Você pode usar as seguintes configurações de saídas de Substance e efeito de camada de textura.

1. Crie um Substance>Textura>Criar Substance e defina o modo como Material irreal. O uso de material irreal permitirá que você veja a textura no visor OGL avançado.
1. Crie saídas para cor base, metálica, aspereza e normal.
1. MODO usa mapas normais OGL. Nas propriedades do Substance, você precisa alterar a direção normal para OpenGL.

   ![](../../../assets/ogl.png)
1. Carregue a predefinição de PBR de Substance. Esta predefinição é uma substituição de octano. Arraste-o para o grupo sombreador.

   [Substance\_PBR.lxp](https://helpx.adobe.com/content/dam/help/en/substance-3d/documentation/integrations/files/162005234/162005272/1/1502792782697/substance-pbr.lxp)
1. Selecione a substituição e arraste as saídas de Substance do Navegador de clipe para a Exibição esquemática. Pegue o nó com a saída do nome do arquivo e conecte-o ao nó de entrada apropriado, ou seja, cor base → cor base.

   ![](../../../assets/connect-6.png)
1. Conecte o restante das saídas de Substance

   ![](../../../assets/outputs-4.png){width="640px"}
