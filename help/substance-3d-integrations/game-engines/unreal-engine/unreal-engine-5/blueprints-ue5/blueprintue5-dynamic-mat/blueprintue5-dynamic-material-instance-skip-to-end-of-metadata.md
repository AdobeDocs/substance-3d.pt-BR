---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/blueprints-ue5/blueprintue5-dynamic-material-instance-skip-to-end-of-metadata.html"
breadcrumb-title: ''
description: Crie instâncias de material dinâmico a partir de materiais de Substance no tempo de execução no Unreal Engine 5 usando Blueprints.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Blueprints - UE5 > Blueprint(UE5) Dynamic Material Instance Skip to end of metadata
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Blueprint(UE5) Instância de material dinâmico Pular para o fim dos metadados
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---


# Blueprint(UE5): Instância de material dinâmico Pular para o fim dos metadados

1. Crie uma variável do tipo Fábrica de instâncias de Substance e defina o valor padrão para a Fábrica de Substance importada.
1. Adicione um nó Criar instância de gráfico e conecte o Substance Instance Fatory à entrada de Fábrica junto com um material pai para agir como um modelo (isso pode ser um dos materiais substance padrão incluídos no plug-in).
1. Crie outra variável para armazenar o objeto Instância de Gráfico do Substance criado na etapa anterior.
1. Use a função “Obter instância de material dinâmico” da instância do gráfico para criar ou obter uma instância de material existente. Deixar as opções Nome e No material principal vazias usará os parâmetros usados ao gerar a instância na etapa 2.
1. Crie uma variável do tipo Material. Esta será a dinâmica da instância do material (MID). Defina o valor de retorno de “Obter instância de material dinâmico” para a variável.

   ![](../../../../../assets/dynamic-material-annotated-1.png)
1. Adicione um nó Definir material e defina o valor da variável MID como a Entrada de material. Para o destino, defina-o como o objeto ao qual deseja aplicar o material.
1. Opcional: Defina quaisquer parâmetros de substância desejados (este exemplo está usando uma ocorrência de gráfico de substância pré-existente e copiando os valores para a nova).
1. Crie um nó de renderização Assíncrono ou Sincronizado e conecte as Instâncias a serem renderizadas à Variável de Instância de Gráfico do Substance.
