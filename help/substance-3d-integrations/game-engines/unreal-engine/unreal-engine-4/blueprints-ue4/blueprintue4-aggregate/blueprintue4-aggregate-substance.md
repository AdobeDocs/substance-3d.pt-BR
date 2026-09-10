---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/blueprints-ue4/blueprintue4-aggregate-substance.html"
breadcrumb-title: ''
description: Combine vários materiais Substance em tempo de execução no Unreal Engine 4 usando nós agregados de Blueprint para workflows avançados.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Blueprints - UE4 > Blueprint(UE4) Aggregate Substance
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Blueprint(UE4) Aggregate Substance
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 0%

---


# Blueprint(UE4): Substance agregado

O novo nó de substância agregada permite que você use dois fatories de instância de substância e crie um novo fatory de instância no tempo de execução, que pode ser usado para criar uma nova instância de gráfico. O que torna isso especial é que você pode conectar texturas de saída de uma das instâncias combinadas de gráfico a imagens de entrada da outra instância combinada de gráfico. Para criar uma instância de gráfico do substance usando essa nova fábrica, consulte nossa documentação sobre instâncias de gráfico do tempo de execução. [Definição de Instância de Material - UE4](https://helpx.adobe.com/substance-3d/unlisted/documentation/integrations/material-instance-definition-157352129.html)

1. Importe Substance que deseja usar.
1. Crie uma variável “AggregateGraphInstance” do tipo **Instância de Gráfico do Substance**.
1. Criar uma variável do tipo **Material** e **Instância de material dinâmica**
1. Crie uma **Criar Conexão Substance** e defina os identificadores de saída e de entrada.
1. Crie a **Fábrica de Instância de Substance Agregação** e defina a Fábrica de Saída e Entrada.
1. Crie uma **Instância de Gráfico** e defina um Nome de Instância.
1. Defina a variável **Instância do gráfico agregado**.
1. Obtenha texturas de substância da Instância do Gráfico Agregado na etapa 7 usando **Obter Texturas de Substance**.
1. Crie uma **Instância de material dinâmico** usando a variável de material da etapa 3 como pai.
1. Defina a variável MID na etapa 3.
1. Defina o material para a malha usando **Definir material** com a variável MID.

   ![](../../../../../assets/a2-3.png){width="800px"}
1. Defina os canais para o material conforme mostrado nos documentos Instância do material dinâmico (etapas 11-19)\
   [Blueprint(UE4): instância de material dinâmico](https://helpx.adobe.com/substance-3d/unlisted/documentation/integrations/blueprint-dynamic-material-instance-152535142.html)

   ![](../../../../../assets/a4-3.png){width="800px"}
