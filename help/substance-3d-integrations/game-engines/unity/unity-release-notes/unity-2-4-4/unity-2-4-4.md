---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-4-4.html"
breadcrumb-title: ''
description: Consulte as notas de versão do plug-in Unity versão 2.4.4 para saber mais sobre novos recursos, aprimoramentos e correções de erros.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.4.4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.4.4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---


# Unity 2.4.4

Lançado em fevereiro de 2020

* Adicionado: Suporte adequado para 2019.3: Corrigidas alterações da API do Unity que quebraram o objeto de script do plug-in Substance. Objetos reformulados para funcionar com atualizações de API 2019.3. Fixo - O uso de material personalizado faz com que o material fique preto ao sair da reprodução
* Corrigido - Falha ao usar a função Duplicate() em um script e depois inserir e sair da reprodução.
* Fixo - aplicação de material, configurações de bloco gráfico e redefinição de sombreador em 2019.3
* Fixo - O sombreador de material HDRP não está atualizando alterações de parâmetro
* Corrigido - o mapa de máscara HDRP não está sendo atualizado
* Fixo - Adicionar parâmetro de string para a função Duplicar
* Corrigido - Corrigir o suporte ao Linux na versão mais recente do Unity Stable
* Corrigido - Problema de endereço do código de bits que precisa ser desativado para o iOS

Problemas conhecidos:

* Renomear o ativo HDRP fará com que o plug-in não gere um mapa de máscara.
* Ao usar o plug-in Substance em um projeto HDRP, o uso da compactação Raw define as texturas em tons de cinza como Alpha 8.
* GameObjects será desmarcado no modo Reproduzir
* Clicar em “Gerar mapas de mip” em um gráfico de Substance no modo de reprodução, a alteração dos parâmetros resulta em um travamento infinito.
