---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/renderers/maxwell/maxwell-substance-painter.html"
breadcrumb-title: ''
description: Exporte texturas de Substance Painter para o renderizador Maxwell usando modelos de saída adequados e configurações de material.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Maxwell > Maxwell - Substance Painter
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Maxwell - Substance Painter
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---


# Maxwell - Substance Painter

O Substance Painter 2020.1 (6.1.0) oferece suporte a Maxwell [Modelos de saída](https://experienceleague.adobe.com/pt-br/docs/substance-3d-painter/using/getting-started/export/export) para metálico/rugosidade e specular/brilho. Você pode simplesmente exportar usando o Modelo de saída Maxwell**.\
O Maxwell 5.1.0** tem uma integração com Substance Painter que permite importar texturas com facilidade e configurar automaticamente um material Maxwell.

## Exportação de texturas

Você pode escolher os Modelos de saída Maxwell (Aspereza metálica) ou Maxwell (Textura reluzente do Specular) para exportar texturas para renderização no Maxwell.

![](../../../assets/maxwell-output.png){width="500px"}

## Aplicar Texturas no Maxwell

Você pode usar a integração de Substance Painter no Maxwell para criar automaticamente um material com os mapas exportados do Substance Painter aplicado.\
Para começar, clique com o botão direito do mouse na Lista de materiais e escolha **Novo>Substance Painter**.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/maxwell-painter?$png$&jpegSize=100&wid=413)

Navegue até o local em que você exportou as texturas de Substance Painter e selecione um dos mapas, como a cor base. Quando você clica em abrir, a integração cria um novo material Maxwell com os mapas atribuídos.\
Se você tiver vários conjuntos de texturas exportados do Substance Painter, a integração usará a convenção de nomenclatura para a textura para atribuir mapas de textura correspondentes.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/image-material?$png$&jpegSize=100&wid=620){width="600px"}

Em seguida, atribua o material ao ativo na cena.

![](../../../assets/assigned.png){width="500px"}

Todos os materiais aplicados usando a integração de Substance Painter.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/materials-assigned?$pjpeg$&jpegSize=300&wid=1511){width="800px"}
