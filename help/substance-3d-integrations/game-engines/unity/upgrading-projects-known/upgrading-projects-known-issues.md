---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/game-engines/unity/upgrading-projects-known-issues.html"
breadcrumb-title: ''
description: Saiba mais sobre como atualizar projetos do Unity com materiais de Substance e problemas conhecidos para evitar durante a migração.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Upgrading ProjectsKnown Issues
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Atualizando projetosProblemas conhecidos
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 1%

---


# Atualizando projetos/problemas conhecidos

>[!WARNING]
>
> O plug-in do Substance 3D para Unity 3.0.0 não oferece suporte à compatibilidade com versões anteriores. Portanto, certifique-se de usar o Unity 2020.3.27x e superior.
> 
> O Unity alterou a arquitetura de compilação padrão para x86 em vez de x86\_64.\
> Scripts não serão executados se fizerem referência a Substance. Você precisará voltar para x86\_64 e a compilação funcionará.

## Problemas conhecidos

* Erro “*Falha de asserção na expressão” ao navegar em pastas do painel.*
  * Esse é um erro que ocorre na extremidade do Unity quando as alterações são feitas na interface do usuário, geralmente alterações em miniatura, devem ser uma mensagem inofensiva.
* *As entradas da imagem parecem estar bloqueadas em 8 bits*
  * Isso foi corrigido na versão 3.8.0-3. O fluxo de trabalho correto seria para os usuários alterarem o formato padrão do Unity para a textura para RGBA64. O plug-in cuidará de enviar corretamente essa informação para o Substance Engine.
