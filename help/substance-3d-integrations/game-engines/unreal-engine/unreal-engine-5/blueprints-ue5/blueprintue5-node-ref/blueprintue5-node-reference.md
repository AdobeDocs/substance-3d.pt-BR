---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/blueprints-ue5/blueprintue5-node-reference.html"
breadcrumb-title: ''
description: Guia de referência para todos os nós de Substance Blueprint disponíveis no Unreal Engine 5 para operações de materiais.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Blueprints - UE5 > Blueprint(UE5) Node Reference
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Referência do Nó Blueprint(UE5)
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '947'
ht-degree: 0%

---


# Blueprint(UE5): referência de nó

## Nós de Substance gerais:

| Nome | Entradas | Descrição |
| --- | --- | --- |
| **GetSubstances** | Entrada: **Material** | Retorna uma matriz de Instâncias de Gráfico do Substance usadas por um material. Se você criar um material que use saídas de textura de duas instâncias de gráfico diferentes, essa função retornará essas duas instâncias de gráfico. |
| **GetSubstanceTextures** | Entrada: **SubstanceGraphInstance** | Retorna uma matriz de todas as texturas habilitadas e atualmente computadas do parâmetro de entrada Instância de Gráfico do Substance. |
| **GetGraphName** | Entrada: **SubstanceGraphInstance** | Retorna o nome do gráfico conforme definido no Designer. |
| **GetFactoryName** | Entrada: **SubstanceGraphInstance** | Retorna o nome da **GraphInstanceFactory** que foi usada para criar a **SubstanceGraphInstance** passada para este nó. |
| **GetSubstanceLoadingProgress** | NENHUM | Retorna um flutuante entre 0 e 1 com a porcentagem de quantas substâncias foram totalmente carregadas. |
| **CreateGraphInstance** | Entrada: **SubstanceInstanceFactory** - A fábrica da qual você deseja criar uma instância de gráfico.Entrada: **GraphIndex** (int) - O índice do gráfico que você deseja criar. Entrada: **InstanceName** (FString) - O nome que você deseja que a nova Instância tenha. | Retorna uma nova instância de gráfico autônoma que persistirá até o aplicativo ser fechado. |
| **DuplicateGraphInstance** | **SubstanceGraphInstance** - A instância do gráfico da qual você deseja criar uma cópia. | Retorna uma nova instância de gráfico autônoma que persistirá até o aplicativo ser fechado. |
| **EnableInstanceOutputs** | Entrada: **SubstanceGraphInstance** - A instância do gráfico que contém a saída para habilitar a Entrada: **OutputIndices** (Matriz int32) - Os índices das saídas que você deseja habilitar. | Se desabilitada anteriormente, cria as saídas de textura de aprovadas em **SubstanceGraphInstance**. Isso tem a mesma funcionalidade que habilitar a saída do Editor de **SubstanceGraphInstance**. *OBSERVAÇÃO: isso não atualizará seu material com a textura recém-criada. Isso precisa ser tratado definindo um parâmetro de amostragem em tempo de execução usando a nova saída.* |
| **DisableInstanceOutputs** | Entrada: **SubstanceGraphInstance** - A instância do gráfico que contém a saída para desabilitar a Entrada: **OutputIndices** (Matriz int32) - Os índices das saídas que você deseja desabilitar | Se habilitada, desabilitará e excluirá a saída de textura para o objeto de gráfico transmitido |
| **CopyInputParameters** | Entrada: **SubstanceGraphInstance** - A instância de gráfico à qual você deseja aplicar valoresEntrada: **SubstanceGraphInstance** - A instância de gráfico da qual você deseja obter os valores | Restaura todos os valores de entrada alterados do parâmetro de entrada Instância de Gráfico do Substance. |
| **ResetInputParameters** | Entrada: SubstanceGraphInstance | Redefinir os valores de entrada de uma Instância de Gráfico do Substance para seus valores padrão |
| **SetGraphInstanceOutputSize** | Entrada: **SubstanceGraphInstance** Entrada: largura - resolução de textura da coordenada XEntrada: Height - resolução de textura da coordenada Y | Define a resolução de textura de todas as saídas geradas a partir desta instância do gráfico com os tamanhos transmitidos pelos parâmetros. Observação - máx. de 2048 no mecanismo da CPUonota - máx. de 4096 no mecanismo da GPU |
| **AsyncRendering** | **SubstanceGraphInstance** | Recalcula texturas de saída da entrada da Instância do Gráfico do Substance. (Sem bloqueio) |
| **SyncRendering** | **SubstanceGraphInstance** | Recalcula texturas de saída da entrada da Instância do Gráfico do Substance. (Bloqueando) |

## Funções Específicas da Instância do Gráfico:

Só pode ser chamado a partir de uma instância de gráfico

| Nome | Entrada | Descrição |
| --- | --- | --- |
| ObterInstânciaDeMaterialDinâmico | Entrada: Nome (String) | Retorna a instância de material dinâmico em tempo de execução de uma substância ou cria uma se não existir uma. Instâncias de material dinâmico são necessárias para a maioria das alterações de valor de tempo de execução a partir das saídas de valor de substância. |
| **GetInputNames** | NENHUM | Retorna uma matriz de Strings contendo todos os nomes de parâmetro de entrada. |
| **GetInputType** | NENHUM | Retorna o tipo de dados associado a esta entrada. |
| **DefinirEntradaInt** | Entrada: **Identificador** (Cadeia de Caracteres)Entrada: **Valores de Entrada** (matriz int) | Altere o valor de uma entrada encontrada pelo identificador. De dentro de um jogo, é necessário renderizar a substância usando **AyncRender** ou **SyncRender** para que as alterações sejam aplicadas. |
| **SetInputFloat** | Entrada: **Identificador** (Cadeia)Entrada: **ValoresDeEntrada** (matriz flutuante) | Altere o valor de uma entrada encontrada pelo identificador. De dentro de um jogo, é necessário renderizar a substância usando **AyncRender** ou **SyncRender** para que as alterações sejam aplicadas. |
| **GetInputInt** | Entrada: **Identificador** (Cadeia de Caracteres) | Retorna uma matriz de inteiros com os valores atuais de um parâmetro de entrada. |
| **GetInputFloat** | Identificador (cadeia de caracteres) | Retorna uma matriz de flutuações com os valores atuais de um parâmetro de entrada. |
| **SetInputBool** | Entrada: **Bool** (Booleano)Entrada: **Identificador** (Cadeia de Caracteres) | Usa um valor booleano para atribuir um tipo de valor de entrada alternável. Anteriormente, isso só era possível definindo um valor int de 1 ou 0 convertido em bool. |
| **GetInputBool** | Entrada: **Identificador** (Cadeia de Caracteres) | Retorna o valor booleano atual de uma entrada. |
| **DefinirCorDeEntrada** | Entrada: **Cor** (LinearColor)Entrada: **Identificador** (FString) | Usa um valor de FLinearColor para atribuir um tipo de valor de entrada de cor. Anteriormente, isso só era possível definindo um valor de flutuação e passando em uma matriz de flutuações. |
| **GetInputColor** | Entrada: Identificador (FString) | Retorna o valor da cor atual no formato UE4. |
| **CreateAggregateSubstanceFactory** | Entrada: **Fábrica de Saída** (SubstanceInstanceFactory)*A fábrica que está criando as saídas que serão usadas como entrada para a fábrica de Entrada.* Entrada: **Índice de Gráfico de Fábrica de Saída** (Inteiro)*Que gráfico dentro da substância você gostaria de usar para combinar.* Entrada: **Fábrica de Entrada** (SubstanceInputFactory)*A fábrica que usa as saídas como imagens de entrada da Fábrica de Saída.*Entrada:**Conexões**(Matriz de SubstanceConnections)*Isso pode ser criado usando o nó de esquema Criar Matriz. Uma conexão de substância é como você pode agregar o nó que as entradas devem vincular a quais saídas.* ** Return (SubstanceInstanceFactory)***Pode ser usado para criar uma instância gráfica da nova instância combinada.* | O novo nó de substância agregada permite que você use dois fatories de instância de substância e crie um novo fatory de instância no tempo de execução, que pode ser usado para criar uma nova instância de gráfico. O que torna isso especial é que você pode conectar texturas de saída de uma das instâncias combinadas de gráfico a imagens de entrada da outra instância combinada de gráfico. Para criar uma instância de gráfico do substance usando essa nova fábrica, consulte nossa documentação sobre instâncias de gráfico do tempo de execução. |
| **SubstanceConnectionStruct** | Entrada: **Identificador de Saída** (FString)*O identificador da saída de textura a ser encadeado em uma entrada.* Entrada: **Identificador de Entrada** (FString) | Usado por Criar Fábrica de Substance de Agregação para especificar como encadear cada textura de saída com novas texturas de entrada. |
