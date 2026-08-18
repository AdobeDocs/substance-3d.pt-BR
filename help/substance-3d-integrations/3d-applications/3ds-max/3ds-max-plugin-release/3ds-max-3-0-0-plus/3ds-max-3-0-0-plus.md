---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-3-0-0-plus.html"
breadcrumb-title: ''
description: Consulte as notas de versão do plug-in 3ds Max versão 3.0.0 e posterior para saber mais sobre novos recursos, aprimoramentos e correções de erros.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds Max Plugin Release Notes > 3ds Max 3.0.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3Ds Max 3.0.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---


# 3ds Max 3.0.0+

## 3ds Max 3.0.4

<b>Adicionado/Atualizado:</b>

* Ícones de plug-in do Substance atualizados com os ícones mais recentes.
* Foi adicionado suporte para envio e recebimento de predefinições usando o conector no plug-in.
* Gerenciador de menus integrado do parâmetro de notificação para substituir o uso da interface principal.

<b>Corrigido:</b>

* Correção de um problema em que os materiais do Substance 2 podiam não renderizar no IR/Produção com o Corona quando o Editor de materiais de ardósia estava aberto e o mapa de textura do Substance 2 estava selecionado.
* Resolvido o problema no qual as atualizações do conector do Sampler estavam criando novos nós Substance2 em vez de atualizar os existentes.
* Resolvido o problema de falha no plug-in 3ds Max ao adicionar um nó Substance2 e garantido que usar a Importação em lote para carregar arquivos .sbsar não abriria mais o editor de script.
* Correção de um problema em que o plug-in 3DSMax 2025 não era carregado devido a um arquivo .dll incompatível ao usar o instalador .msi.

## 3ds Max 3.0.2

<b>Adicionado/Atualizado:</b>

* Gerenciamento padronizado de ícones no plug-in Substance, incorporando todos os ícones existentes em arquivos qrc e rcc, alinhando-se aos métodos preferidos da Autodesk e garantindo um carregamento consistente no painel gráfico SBSAR.
* A capacidade de resposta da janela de configurações de Substance no plug-in foi aprimorada para garantir que os campos de entrada e suas descrições se ajustem corretamente ao ajustar o tamanho da janela.
* O plug-in Substance agora é compatível com o Corona 11.

<b>Corrigido:</b>

* Correção de um problema em que a aspereza de Cor do brilho e brilho não se conectava automaticamente em materiais de raio V. Agora, ambas as propriedades serão vinculadas automaticamente ao criar um fluxo de trabalho no V-Ray e no Arnold.
* Correção de um problema de interface do usuário no plug-in em que o ajuste da configuração Limite de núcleos da CPU exibia incorretamente valores de dois dígitos se o valor salvo fosse um único dígito.
* Correção de um erro de renderização no console para o plug-in 3ds Max v3.0.0 relacionado ao recurso de compatibilidade de Substance. Agora, os nós do substance criados usando o menu Importar lote de Substance são renderizados conforme esperado.
