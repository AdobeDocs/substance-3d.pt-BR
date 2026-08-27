---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-4-0.html"
breadcrumb-title: ''
description: Consulte as notas de versão do plug-in Unity versão 2.4.0 para saber mais sobre novos recursos, aprimoramentos e correções de erros.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.4.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.4.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---


# Unity 2.4.0

>[!WARNING]
>
> O Unity alterou a arquitetura de compilação padrão para x86 em vez de x86\_64.\
> Scripts não serão executados se fizerem referência a Substance. Você precisará voltar para x86\_64 e a compilação funcionará.

## Novos recursos:

* Suporte a projeto HDRP adicionado (visualização)
* Preferências adicionadas no menu Substance
* Adicionada a capacidade de definir a configuração de importação da resolução de Substance padrão
* Adição da capacidade de definir a compactação normal padrão
* Capacidade adicionada de gerar todas as saídas em uma importação de um Substance
* Suporte para saídas + saídas personalizadas com o mesmo uso
* Configurações de resolução da plataforma adicionadas
* Correções de erros de suporte ao IL2CPP adicionadas

### Correções de erros:

* Correção de um erro em que abrir o Substance Source no Mac OS gerava um erro de Linux
* Redução do tempo necessário para trocar de plataforma. A conversão de textura para plataformas móveis agora é feita na compilação, em vez de ao alternar a plataforma de destino.
* Erro de falha de asserção ao importar sbsar
* Atualizar projetos usando o .NET 3.5 faz com que os materiais do substance sejam quebrados
* Fonte de Substance não suportada na caixa de diálogo do linux que aparece no OS X
* A alteração do nome do gráfico destrói pré-fabricações e arquivos de cena no modo de serialização ForceText
* materiais de Substance com várias saídas usando o mesmo uso quebrarão Plug-in não suporta saídas personalizadas em sbsar

### Problemas conhecidos:

* Ao atualizar um projeto de 2017-2018/2019, depois que o usuário importa o plug-in Substance, o Unity deve ser reiniciado para que o projeto seja atualizado.\
  Solução alternativa: crie um pacote de ativos/projeto e importe esse pacote para um projeto mais recente com o plug-in 2.4.0. Os arquivos de Substance devem ser convertidos corretamente.
* O Unity alterou a arquitetura de compilação padrão para x86. Atualmente, o plug-in Substance só é compatível com x86\_64.

**Não Há Mais Suporte Total:**

* O Substance Live Link foi removido do pacote da Asset Store. (O pacote ainda pode ser baixado do Substance share)
