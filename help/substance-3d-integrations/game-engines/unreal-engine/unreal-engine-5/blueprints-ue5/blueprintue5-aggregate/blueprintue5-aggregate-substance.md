---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/blueprints-ue5/blueprintue5-aggregate-substance.html"
breadcrumb-title: ''
description: Combine vários materiais Substance em tempo de execução no Unreal Engine 5 usando nós agregados de Blueprint para workflows avançados.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Blueprints - UE5 > Blueprint(UE5) Aggregate Substance
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Blueprint(UE5) Aggregate Substance
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---


# Blueprint(UE5): Substance agregado

1. Use o nó “Create Aggregate Substance Fatory” (Criar fábrica de agregada) e defina o Output and Input Fatory (Fábrica de saída e de entrada). A fábrica de saída deve ter um mapa de textura que seria usado como uma imagem de entrada nos parâmetros de fábrica de entrada.
1. Crie objetos SubstanceConnection para cada textura de saída usada como uma entrada com os nomes dos valores correspondentes (o nome de saída do gráfico de saída e o nome do parâmetro de entrada do gráfico de entrada)
1. Adicione um nó Criar instância de gráfico e conecte o resultado do nó “Criar fábrica de Substance agregada” à entrada de fábrica junto com um material pai para agir como um modelo (isso pode ser um dos materiais padrão\_substance incluídos no plug-in).
1. Crie uma variável Instância de Gráfico do Substance e armazene o resultado do nó anterior.
1. Opcional: Defina quaisquer parâmetros de substância desejados (este exemplo está definindo uma nova resolução para as saídas do gráfico).
1. Crie um nó de renderização Assíncrono ou Sincronizado e conecte as Instâncias a serem renderizadas à Variável de Instância de Gráfico do Substance.
1. Use a função “Obter instância de material dinâmico” da instância do gráfico para criar ou obter uma instância de material existente. Deixar as opções Nome e No material principal vazias usará os parâmetros usados ao gerar a instância na etapa 3.
1. Adicione um nó Definir material e defina o valor da variável MID como a Entrada de material. Para o destino, defina-o como o objeto ao qual deseja aplicar o material.
