---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/material-instance-definition-ue5.html"
breadcrumb-title: ''
description: Crie Definições de instância de material com materiais de Substance no Unreal Engine 5 para otimizar o desempenho de renderização da GPU.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Material Instance Definition - UE5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Definição de Instância de Material - UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '271'
ht-degree: 0%

---


# Definição de Instância de Material - UE5

Você pode usar instâncias de material UE5 com Substance. Isso salvará uma grande etapa no processo de renderização da GPU, pois não carregará novos materiais no processo. Um MID pode ser criado em tempo de execução ou no editor. Com a versão 5.0.0, adicionamos suporte total para instanciação de material.

## Criação de uma ocorrência de material no editor

1. Clique com o botão direito do mouse no material UE5 criado pela substância e escolha “Criar ocorrência de material”. Isso cria um material de Instância UE5.

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/screen-shot-2022-03-31-at-6-07-08-pm?$png$&jpegSize=300&wid=1472)
1. Clique com o botão direito do mouse na fábrica de instâncias do substance e escolha “Criar uma instância de gráfico”. Isso criará uma instância do gráfico e outro material UE5. Exclua o material UE5 recém-criado, pois ele não será usado.

   ![](../../../../assets/screen-shot-2022-03-31-at-6-10-38-pm.png)
1. Clique duas vezes na instância do material criada na etapa 1 e ative os parâmetros de Textura para todos os mapas.
1. Defina a textura para a nova textura INST criada na etapa 2. Isso definirá a ocorrência do material para usar os mapas de saída do substance a partir do gráfico de ocorrência.

   ![](../../../../assets/screen-shot-2022-03-31-at-6-13-18-pm.png)

Agora você tem uma instância de material UE5 que está usando um conjunto específico de texturas do substance. Esta é uma forma mais otimizada de trabalhar com múltiplas substâncias num projeto UE5. Para saber como criar um MID usando o blueprint, verifique esta página. [Blueprint(UE5): Instância de Material Dinâmico](https://helpx.adobe.com/substance-3d/unlisted/documentation/integrations/blueprint-dynamic-material-instance-152535142.html)
