---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/corona/corona-for-3ds-max.html"
breadcrumb-title: ''
description: Use materiais de Substance com o renderizador Corona no 3ds Max usando o fluxo de trabalho Specular/Textura reluzente e os mapas necessários.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Corona > Corona for 3ds Max
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Corona para 3ds Max
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '194'
ht-degree: 0%

---


# Corona para 3ds Max

## Substance no plug-in Maya

![](../../../assets/scene-001v03.jpg)

## Corona 1,6 - 6

Usando o [plug-in 3ds Max](../../../3d-applications/3ds-max/3ds-max.md), você pode escolher Corona no menu Substance para configurar automaticamente o material Corona com entradas de textura Substance.

![](../../../assets/corona.png){width="500px"}

## Corona 7 - 9

Para a renderização Corona 7 e superior, selecionar “Substance para Corona” com o nó Substance 2 selecionado criará uma rede para o Material físico Corona.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/corona-physical-material?$png$&jpegSize=200&wid=857)

* **LiftGamaGain** é criado entre a saída da Cor Base e a entrada da Cor Base. Um valor de gama de 0,455 é usado para corrigir a diferença de cor.
* **CoronaNormal** é criado entre a saída Normal e a entrada de Relevo Base, e também entre a saída Coat Normal e a entrada Clearcoat Bump. Nenhuma configuração é alterada, mas as modificações para o normal podem ser feitas aqui.
* **CoronaMix** é criada entre a saída da Cor do brilho e a entrada da Cor do brilho. Uma Quantidade de mix de 0 é definida e um multiplicador de 2 é definido para a Camada base. Os usuários podem ajustar o valor do Valor de mixagem para controlar o brilho.
