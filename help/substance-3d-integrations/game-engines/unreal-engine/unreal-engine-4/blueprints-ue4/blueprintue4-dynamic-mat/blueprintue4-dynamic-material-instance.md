---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/blueprints-ue4/blueprintue4-dynamic-material-instance.html"
breadcrumb-title: ''
description: Crie instâncias de material dinâmico a partir de materiais de Substance no tempo de execução no Unreal Engine 4 usando Blueprints.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Blueprints - UE4 > Blueprint(UE4) Dynamic Material Instance
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Instância de material dinâmico Blueprint(UE4)
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---


# Blueprint(UE4): Instância de material dinâmico

Você pode criar uma ocorrência de Gráfico do Substance para criar uma ocorrência de gráfico dinâmico no tempo de execução.

1. Crie uma variável do tipo Fábrica de instâncias de Substance e defina o valor padrão para a Fábrica de Substance importada.
1. Adicione um nó Criar instância de gráfico e conecte o Alocador de instância de Substance na entrada do Alocador de fábrica. Defina um Nome de instância.
1. Crie outra variável do tipo Fatory de Instância de Substance. Isso manterá referências ao material da substância dinâmica.
1. Defina a variável para o material dinâmico da substância com o valor de retorno do nó Criar instância de gráfico.
1. Crie uma variável do tipo Material. Esse será o modelo do material. No Navegador de conteúdo, faça uma duplicata do material UE4 gerado pelo Substance. Defina este material duplicado como a entrada para a variável de modelo de material.
1. Adicione uma Instância de material dinâmico e defina a variável Modelo de material como a principal.

   ![](../../../../../assets/rt-01.png){width="800px"}
1. Crie uma variável do tipo Material. Esta será a dinâmica da instância do material (MID). Defina o valor de retorno da Instância do material dinâmico para a variável.

   ![](../../../../../assets/rt-02.png){width="800px"}
1. Adicione um nó Definir material e defina o valor da variável MID como a Entrada de material. Para o destino, defina-o como o objeto ao qual deseja aplicar o material.
1. Crie uma variável do tipo Nome. Essa variável manterá o nome dos canais definidos no material. Inicialize com um valor de “NONE”
1. Adicione um nó Obter texturas de Substance e defina a Instância do gráfico para a variável Instância do gráfico dinâmico.
1. Adicione um nó de Loop For. Aqui você executa o loop pelas texturas de Substance. Tome o resultado de Get Substance Textures como a matriz de entrada.

   ![](../../../../../assets/rt-03.png){width="800px"}
1. Adicione um nó Substance Get Channel com o elemento de matriz do loop for como entrada.
1. Adicione um nó de sequência. Aqui, primeiro executaremos o resultado do nó Obter canal.
1. Adicione um Switch em ESubChannelType após a Sequência Then 0 com o valor de retorno Get Channel como a Seleção. Aqui nós verificamos os nomes dos canais.
1. Defina a variável MID Name para os nomes de canal no Material de Substance duplicado na etapa 5. *Veja a imagem do material.*
1. No nó Sequência Em seguida, 1, você configurará o processo de atribuição dos nomes dos canais ao material dinâmico.
1. Obtenha a variável de nome MID e adicione um nó de string igual com um valor de “NONE”. Esse é o valor que inicializará a variável.
1. Adicione um nó Branch com a Condição do nó Equal.
1. Adicione um valor de parâmetro de textura de conjunto de Substance. O destino é a variável MID e o nome do parâmetro é a variável de nome MID. O Valor é o Elemento Array do Nó ForEachLoop.

![](../../../../../assets/material-1.png){width="800px"}
