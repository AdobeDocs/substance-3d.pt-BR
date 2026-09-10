---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-6-0.html"
breadcrumb-title: ''
description: Consulte as notas de versão do plug-in Unity versão 2.6.0 para saber mais sobre novos recursos, aprimoramentos e correções de erros.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.6.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.6.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---


# Unity 2.6.0

Lançado em 7 de junho de 2021

Atualizado/adicionado:

* Novo fluxo de trabalho para acessar o Substance Source! A ação Substance Source agora acessa a guia Origem no Iniciador de Substance, permitindo que os ativos sejam enviados diretamente para o Unity
* As informações da versão do plug-in podem ser copiadas para a área de transferência
* “Gerar ao carregar” removido das Configurações de destino

Correções:

* Em projetos HDRP, o modo de Deslocamento reverterá para o valor padrão (Teste) quando for feita uma alteração na configuração do material
* O tamanho da resolução não é exibido na janela Inspetor
* Não é possível instalar o plug-in nas versões 2020.2 e posteriores do Unity

Problemas conhecidos:

* O erro de acesso negado e/ou falha ocorre ao atualizar o plug-in das versões anteriores 2.5.4 e anteriores
  * Solução alternativa: as versões 2.5.4 e anteriores do plug-in precisam ser desinstaladas das versões 2020.2 e posteriores do projeto Unity antes de instalar a versão 2.6.0 do plug-in
* As visualizações de Textura para arquivos de imagem não serão exibidas no inspetor quando o plug-in Substance for instalado
  * A origem desse problema existe no Unity e está planejada para ser corrigida pelo Unity em suas versões 2021.2 (atualmente em beta)
