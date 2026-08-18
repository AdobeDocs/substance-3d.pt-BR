---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/3d-applications/maya/maya-plugin-release-notes/maya-3-0-0-plus.html"
breadcrumb-title: ''
description: Revise as notas de versão do plug-in Maya versão 3.0.0 e posterior para saber mais sobre novos recursos, melhorias e correções de erros.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds Max Plugin Release Notes > Maya 3.0.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Maya 3.0.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---


# Maya 3.0.0+

## Maya 3.0.3

<b>Adicionado/Atualizado:</b>

* O sistema de cache do plug-in do Maya foi aprimorado para armazenar em cache apenas uma vez na criação inicial da rede, com o rearmazenamento em cache manual habilitado.
* Foi fornecida uma opção para alterar o local da pasta “substance” no plug-in Maya.
* O sistema de importação de fluxo de trabalho do plug-in Maya foi atualizado para garantir compatibilidade com a atualização da Autodesk para o Python 3.12.
* Ícones de plug-in do Substance atualizados com os ícones mais recentes.
* Foi adicionado suporte para envio e recebimento de predefinições usando o conector no plug-in.

<b>Corrigido:</b>

* Correção de um problema em que carregar/descarregar o plug-in Substance para Maya produz uma tela de erro e falha.
* Correção de problemas de cache, garantindo especificamente que os arquivos .exr fizessem referência corretamente e reduzindo os congelamentos relacionados ao cache em cenas grandes.
* Resolvido um problema em que a visualização de material na janela Amostra não era exibida quando um arquivo SBSAR era carregado no plug-in do Maya.
* Resolvido o problema em que o conector não recebia o arquivo SBSAR se pelo menos um SBSAR já estivesse no Hypershade.
