---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/sharing-sbsar-files-between-projects.html"
breadcrumb-title: ''
description: Compartilhe arquivos Substance SBSAR entre projetos do Unity enquanto preserva os ajustes de parâmetro usando arquivos predefinidos.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity >Sharing sbsar Files Between Projects
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Compartilhamento de arquivos sbsar entre projetos
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---


# Compartilhamento de arquivos sbsar entre projetos

É possível compartilhar arquivos .sbsar entre projetos e computadores enquanto mantém os mesmos ajustes de parâmetro com o uso de arquivos .sbsprs.

Depois que o material no projeto original for modificado para as configurações que serão compartilhadas, navegue até as configurações predefinidas no painel inspetor. Nas configurações de predefinição, crie uma nova predefinição e nomeie-a. Essa nova predefinição nomeada aparecerá na lista de predefinições para esse material. Depois disso, exporte a predefinição para salvá-la localmente.

Ao usar o arquivo .sbsar em outro projeto ou computador, inclua também o arquivo de predefinição exportado. Depois que o sbsar for importado para o projeto do Unity, navegue até as configurações predefinidas e escolha a opção de importação. Selecione o arquivo de predefinição da etapa anterior e importe-o. Uma predefinição com as configurações do projeto anterior deve ser adicionada à lista de predefinições.

Repita o processo para todos os materiais que estão sendo compartilhados.
