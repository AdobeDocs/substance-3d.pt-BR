---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/plugin-settings-ue5.html"
breadcrumb-title: ''
description: Defina as configurações do plug-in Substance no Unreal Engine 5 por meio de Configurações do projeto para personalizar o comportamento do plug-in.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Plugin Settings - UE5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Configurações do plug-in - UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---


# Configurações do plug-in - UE5

Para acessar as configurações, vá para Editar > Configurações do projeto, role para baixo até a categoria Plug-ins e clique em Substance.

![](../../../../assets/screen-shot-2022-03-31-at-5-50-29-pm.png)

## Orçamento de hardware

O orçamento de memória é a quantidade máxima de memória a ser usada para o mecanismo de Substance. Pode ser aumentado para melhorar a velocidade de processamento do Substance, mas consumirá mais recursos do sistema. (Nem sempre um aumento útil no nível do projeto).

Os núcleos da CPU determinam quantos núcleos o mecanismo de Substance pode usar. Isso inclui núcleos físicos e hyper threads. (Se o número atribuído for maior que os núcleos disponíveis em um sistema, o padrão será usar todos os núcleos disponíveis.

## Cozinhar

A contagem do Nível de mapeamento removida durante o cozimento alterará a forma como as texturas são criadas para um pacote. Essa configuração pode melhorar muito os tempos de carregamento e reduzir o tamanho do pacote, pois os níveis de mip de textura maiores não precisarão mais ser carregados. A resolução mais baixa / LODs menores serão carregados e o mais alto será padronizado por UE5. Os Substance são então processados através do mecanismo de Substance e atualizados em tempo de execução com os LODs de alta resolução.

O Substance Engine pode ser CPU ou GPU. O mecanismo da GPU permitirá criar texturas 4K. O mecanismo da CPU está limitado a 2K.

## Otimização:

Isso limita quantas substâncias assíncronas podem ser passadas para o mecanismo de substâncias em cada lote. Números mais baixos acelerarão a rapidez com que uma tarefa assíncrona será concluída e atualizada, em que números mais altos renderizarão em lote e processarão vários Substance de cada vez. (Quanto maior o número, mais atualizações de textura cortada se tornam porque o tempo entre as atualizações é maior).

## Renderização assíncrona/sincronizada

A renderização de sincronização está bloqueando a chamada de renderização. Isso passará uma instância de gráfico de Substance para o mecanismo de Substance a ser recalculado, mas interromperá a execução até que o mecanismo de Substance tenha terminado de processar o Substance antes de continuar com qualquer execução de código adicional. O resultado também será atualizado na tela assim que o processo for concluído.

O Async adicionará seu gráfico a uma fila e enviará vários gráficos ao mecanismo de Substance de cada vez (definido nas configurações de Substance) na atualização do plug-in. Ao contrário da renderização de sincronização, assim que são enviados, o programa continua funcionando normalmente, em vez de esperar em torno do mecanismo de Substance para ser concluído. Quando o mecanismo Substance tiver terminado esse lote, ele envia os resultados de volta, nós os aplicamos às saídas, e iniciamos outro lote.
