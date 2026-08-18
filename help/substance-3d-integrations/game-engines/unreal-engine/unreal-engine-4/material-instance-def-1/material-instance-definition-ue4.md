---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/material-instance-definition-ue4.html"
breadcrumb-title: ''
description: Crie Definições de instância de material com materiais de Substance no Unreal Engine 4 para otimizar o desempenho de renderização da GPU.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Material Instance Definition - UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Definição de Instância de Material - UE4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---


# Definição de Instância de Material - UE4

Você pode usar instâncias de material UE4 com Substance. Isso salvará uma grande etapa no processo de renderização da GPU, pois não carregará um novo material para processar. Um MID pode ser criado em tempo de execução ou no editor. Com a versão 4.24.0.3, adicionamos suporte total para instanciação de material e introduzimos um novo fluxo de trabalho de modelo de material com saídas numéricas com suporte do Substance Engine. Os modelos de material permitem que você defina exatamente como deseja configurar os sombreadores de material de Substance em UE4.

Ao importar um arquivo sbsar, você pode escolher com qual modelo deseja trabalhar.

![](../../../../assets/ue4-material-templates.png)

Enviamos modelos para trabalhar com materiais de deslocamento, refração e alinhados mundialmente que possuem controles incorporados para ajustar a divisão em blocos gráficos, o tamanho da textura, o deslocamento e os parâmetros emissivos. O sistema de modelos de material também permite que você forneça seus próprios modelos personalizados.

![](../../../../assets/ue4-material-instance-params.png)

## Criação de uma ocorrência de material no editor

1. Clique com o botão direito do mouse no material UE4 criado pela substância e escolha “Criar ocorrência de material”. Isso cria um material com instância UE4.

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/01-12?$png$&jpegSize=100&wid=592){width="560px"}
1. Clique com o botão direito do mouse na fábrica de instâncias do substance e escolha “Criar uma instância de gráfico”. Isso criará uma instância do gráfico e outro material UE4. Exclua o material UE4 recém-criado, pois ele não será usado.

   ![](../../../../assets/02-10.png){width="300px"}
1. Clique duas vezes na instância do material criada na etapa 1 e ative os parâmetros Textura para todos os mapas.
1. Defina a textura para a nova textura INST criada na etapa 2. Isso definirá a ocorrência do material para usar os mapas de saída do substance a partir do gráfico de ocorrência.

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/03-6?$png$&jpegSize=200&wid=1011){width="800px"}

Agora você tem uma instância de material UE4 que está usando um conjunto específico de texturas do substance. Esta é uma maneira mais otimizada de trabalhar com várias substâncias em um projeto UE4. Para saber como criar um MID usando o blueprint, verifique esta página. [Blueprint(UE4): instância de material dinâmico](https://helpx.adobe.com/substance-3d/unlisted/documentation/integrations/blueprint-dynamic-material-instance-152535142.html)
