---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/plugin-settings-ue4.html"
breadcrumb-title: ''
description: Defina as configurações do plug-in Substance no Unreal Engine 4 por meio das Configurações do projeto para personalizar o comportamento do plug-in.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Plugin Settings - UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Configurações do plug-in - UE4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 0%

---


# Configurações do plug-in - UE4

Para acessar as configurações, vá para Editar > Configurações do projeto, role para baixo até a categoria Plug-ins e clique em Substance.

![](../../../../assets/settings-36.png){width="400px"}

## Orçamento de hardware

O orçamento de memória é a quantidade máxima de memória a ser usada para o mecanismo do substance. Pode ser aumentado para melhorar a velocidade de processamento de substâncias, mas consumirá mais recursos do sistema. (Nem sempre um aumento útil no nível do projeto).

Os núcleos da CPU correspondem ao número de núcleos que o mecanismo de Substance pode usar. Isso inclui núcleos físicos e hyper threads. (Se o número atribuído for maior que os núcleos disponíveis em um sistema, o padrão será usar todos os núcleos disponíveis.

## Cozinhar

A contagem do Nível de mapeamento removida durante o cozimento alterará a forma como as texturas são criadas para um pacote. Essa configuração pode melhorar muito os tempos de carregamento e reduzir o tamanho do pacote, pois os níveis de mip de textura maiores não precisarão mais ser carregados. A resolução mais baixa / LODs menores serão carregados e o mais alto será padronizado pelo UE4. As substâncias são então processadas através do motor da substância e atualizadas em tempo de execução com os LD de alta resolução.

O Substance Engine pode ser CPU ou GPU. O mecanismo da GPU permitirá criar texturas 4K. O mecanismo da CPU está limitado a 2K.

## Geração padrão:

O Modo de Geração de Substance (SGM) controla como as texturas são geradas. Essa é uma configuração global para Substance. O SGM pode ser alterado por Substance na fábrica de Substance.

**Assado por SGM**: prepara as texturas da substância. Você perde a capacidade de alterar parâmetros no tempo de execução.

**SGM na Sincronização de Carregamento**: bloqueia o aplicativo enquanto os Substance estão sendo carregados.

**SGM em Sincronização de Carga e Cache**: armazena em cache um resultado intermediário da textura no disco.

**SGM em Carregar Assíncrono**: sem bloqueio. Os Substance são gerados em segundo plano.

**SGM em Carregar Assíncrono e Cache**: armazena em cache um resultado intermediário da textura no disco.

***O Padrão da Plataforma é Carregar Assíncrono e Cache***

## Fábrica de Substance

Para alterar o SGM de um Substance, clique com o botão direito em Substance Fatory>Ações de ativo>Edição em massa via Matriz de propriedades. Você pode então alterar o SGM.

![](../../../../assets/sgm.png){width="800px"}

## Otimização:

Isso limita quantas substâncias assíncronas podem ser passadas para o mecanismo de substâncias em cada lote. Números mais baixos acelerarão a rapidez com que uma tarefa assíncrona será concluída e atualizada, onde números mais altos renderizarão em lote e processarão várias substâncias de uma vez. (Quanto maior o número, mais atualizações de textura cortada se tornam porque o tempo entre as atualizações é maior).

## Renderização assíncrona/sincronizada

A renderização de sincronização está bloqueando a chamada de renderização. Isso passará uma instância do gráfico do substance para o mecanismo do substance a ser recalculado, mas interromperá a execução até que o mecanismo do substance termine de processar o substance antes de continuar com qualquer execução de código adicional. O resultado também será atualizado na tela assim que o processo for concluído.

O Async adicionará seu gráfico a uma fila e enviará vários gráficos ao mecanismo do substance de cada vez (definido nas configurações do substance) na atualização do plug-in. Ao contrário da renderização de sincronização, assim que são enviados, o programa continua funcionando normalmente, em vez de esperar em torno do mecanismo do substance ser concluído. Quando o mecanismo do substance tiver terminado esse lote, ele envia os resultados de volta, nós os aplicamos às saídas, e iniciamos outro lote.
