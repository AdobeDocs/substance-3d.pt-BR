---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/3d-applications/maya/maya-plugin-release-notes/maya-2-2-1.html"
breadcrumb-title: ''
description: Consulte as notas de versão do plug-in Maya versão 2.2.1 para saber mais sobre novos recursos, melhorias e correções de erros.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Maya Plugin Release Notes > Maya 2.2.1
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Maya 2.2.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 0%

---


# Maya 2.2.1

Versão Do Maya 2.2.1:

* Atualizar Substance Engine para 8.3.0
* Adição de suporte nativo para Arnold, eliminando a necessidade de cache para disco
* Isso pode ser usado após ativar as extensões de renderização nas configurações e reiniciar o Maya
* As versões compatíveis são:
* Maya 2017 - MtoA 3.1.0/Arnold 5.2.0
* Maya 2018 - MtoA 4.0.0/Arnold 6.0.0, MtoA 4.2.0/Arnold 6.2.0
* Maya 2019 - MtoA 4.0.0/Arnold 6.0.0, MtoA 4.2.0/Arnold 6.2.0, MtoA 5.0.0/Arnold 7.0.0
* Maya 2020 - MtoA 4.0.0/Arnold 6.0.0, MtoA 4.2.0/Arnold 6.2.0, MtoA 5.0.0/Arnold 7.0.0
* Maya 2022 - MtoA 4.2.1/Arnold 6.2.0, MtoA 5.0.0/Arnold 7.0.0
* Diretório de instalação atualizado no Windows e no MacOS
* Os binários no MacOS/Windows agora são assinados usando certificados Adobe
* Os alternadores de canal agora estão ocultos quando o autor da sbsar é Allegorítmico ou Adobe, em vez de apenas Allegorítmico
* Adicionada nova interface de usuário de fluxo de trabalho, com funcionalidade adicional para duplicação, substituição, renomeação e exclusão de fluxos de trabalho

Foram adicionados os seguintes novos comandos de script:

substancemaya

substanceGetEnableRenderingExtensions

substanceSetEnableRenderingExtensions

substanceWorkflow.py

substanceWorkflowIsReadOnly

substanceWorkflowRenameWorkflow

substanceWorkflowDuplicateWorkflow

substanceWorkflowOverwriteWorkflow

substanceWorkflowRemoveWorkflow

Correções de erros:

* Corrigir o erro ao abrir a caixa de diálogo Configurações
* As funções de fluxo de trabalho não falham mais quando um pyc era gerado

Esta versão foi lançada para o Maya 2017, 2018, 2019, 2020 e 2022 no Linux, MacOS e Windows, e para o Maya LT 2018, 2019 e 2020 no MacOS e no Windows
