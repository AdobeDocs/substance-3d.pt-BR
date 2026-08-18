---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/guides/error-and-warning-messages.html"
breadcrumb-title: ''
description: Guia de referência para todas as mensagens de erro e aviso que podem aparecer ao assar com software Substance.
helpx_creative_field: ""
helpx_description: bakers > Guides > Error and Warning Messages
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Mensagens de Erro e Aviso
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 0%

---


# Mensagens de Erro e Aviso

Abaixo está a lista de todas as mensagens de erro que podem aparecer ao assentar com o software Substance.

## Qualquer padeiro

| *Mensagem* | *Descrição* |
| --- | --- |
| Padeiro não disponível. | Essa mensagem de erro geralmente é seguida por mensagens de erro adicionais, geralmente relacionadas a problemas de GPU. Isso pode acontecer se a GPU for muito antiga e não atender aos [requisitos técnicos](https://www.allegorithmic.com/products/tech-specs) do software. |
| O conjunto UV [X] não existe. | O Baker tentou trabalhar com um conjunto UV dado que não está presente na malha de baixo-poli. |
| Não é possível carregar a cena da URL. | Essa mensagem indica que o padeiro não conseguiu carregar o arquivo de malha, geralmente a malha em alta pressão. Algumas razões podem ser a origem desta mensagem:<ul data-preserve-html="true"><li data-preserve-html="true">O arquivo de malha referenciado não existe mais.</li><li data-preserve-html="true">O arquivo de malha está corrompido ou danificado e não pode ser lido.</li><li data-preserve-html="true">No momento, a malha está sendo editada por outro aplicativo e não pode ser lida.</li></ul> |

## UV para SVG Baker

| *Mensagem* | *Descrição* |
| --- | --- |
| Não foi possível localizar UVs para malha [nome da malha]. | Nenhum UV foi encontrado em relação a uma malha específica. Isso pode acontecer se várias malhas forem importadas, mas apenas algumas delas tiverem UVs. |
| A cena não tem UVs. Cancelando cozimento. | Se nenhuma malha na cena tiver UVs, o processo de cozimento será cancelado. |

## Position Baker

| *Mensagem* | *Descrição* |
| --- | --- |
| A malha [nome da malha] não tem posições. | A malha de baixa poli não tem posições de vértice. |
| A malha [nome da malha] não tem UVs para uv definido [X]. | O Baker tentou trabalhar com um conjunto UV dado que não está presente na malha de baixo-poli. |

## Qualquer padeiro “De malha”

| *Mensagem* | *Descrição* |
| --- | --- |
| Não foi possível localizar normais de vértice na malha [nome da malha]. | Nenhum normal de vértice foi encontrado na malha fornecida. Normalmente nunca acontece porque os normais de vértice são recalculados se a malha não os tiver. Isso pode acontecer por causa de um plug-in de espaço tangente personalizado defeituoso. |
| Não foi possível localizar tangentes de vértice na malha [nome da malha]. | Igual como acima. |
| Não foi possível localizar binormais de vértice na malha [nome da malha]. | Igual como acima. |
| Não foi possível encontrar cores de vértice na malha [nome da malha]. | Nenhuma cor de vértice foi encontrada na malha fornecida. Isso pode acontecer se pelo menos uma sub-malha na malha de alto polígono não tiver nenhuma cor de vértice definida. |
| Não há dados suficientes no poli alto para usar o padeiro selecionado. Cancelando cozimento. | Precedido por pelo menos uma das mensagens acima. Normalmente, se apenas um pouco de dados estiver faltando na cena (por exemplo: apenas uma malha em uma cena com alto índice de polígonos não tem cores de vértices), o processo de cozimento preenche os dados ausentes com zeros e continua cozinhando. Se houver muitos dados ausentes, esta mensagem será enviada e o processo de preparo será interrompido. |

## Textura transferida da malha

| *Mensagem* | *Descrição* |
| --- | --- |
| Falha ao carregar textura detalhada. | Não foi possível carregar a textura definida nas configurações do padeiro. Pode ser porque o arquivo está realmente ausente no disco ou porque está corrompido e não pode ser lido. |
