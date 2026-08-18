---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-5-2.html"
breadcrumb-title: ''
description: Consulte as notas de versão do plug-in Unity versão 2.5.2 para saber mais sobre novos recursos, aprimoramentos e correções de erros.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.5.2
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.5.2
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 0%

---


# Unity 2.5.2

Lançado em 23 de julho de 2020

Adicionado:

* Função “IsProcessing()” que indica se o renderizador está ocupado ou Ocioso (não ocupado)

Corrigido:

* Não exibe mais um erro ao definir as configurações de 2048 clamp e 4096 target
* As propriedades de material serão mantidas ao atualizar para HDRP e/ou URP a partir do padrão
* Scripts que alteram materiais de Substance funcionarão conforme o esperado ao implantar em dispositivos móveis
* O canal vermelho não é mais copiado para o Alpha e o Alpha para o branco, como padrão
* Falha ao alterar as configurações de destino no Mac
* Erro NullReferenceException removido ao criar Material de Unidade
* Erro removido ao sair do Modo de reprodução após editar propriedades de divisão em blocos gráficos
* Ativar instância de GPU pode ser ativado
* Os materiais que usam Transparência não desaparecerão ou ficarão pretos incorretamente quando o Modo de reprodução existente
* Os materiais do Substance não serão destruídos no projeto HDRP ao atualizar o plug-in
