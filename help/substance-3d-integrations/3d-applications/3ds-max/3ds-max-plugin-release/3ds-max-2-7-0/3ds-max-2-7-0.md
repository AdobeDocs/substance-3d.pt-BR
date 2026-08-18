---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-2-7-0.html"
breadcrumb-title: ''
description: Consulte as notas de versão do plug-in 3ds Max versão 2.7.0 para saber mais sobre novos recursos, melhorias e correções de erros.
helpx_creative_field: ""
helpx_description: Substance 3D Integrations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max 2.7.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---


# 3ds Max 2.7.0

<b>Adicionado/Atualizado:</b>

* Atualização do mecanismo Substance para a versão 9 do plug-in 3ds Max, aprimorando o desempenho e a compatibilidade.

<b>Corrigido:</b>

* Correção de um problema de falha nas versões 2019, 2022, 2023 e 2024 do 3ds Max, em que arrastar um nó Substance 2 para o Editor de material de folha fazia com que o programa falhasse. O nó Substance 2 agora pode ser arrastado e solto com segurança no Editor de material de ardósia.
* Correção de um problema no plug-in Substance para o 3ds Max, em que a seleção de &#39;Substance para Arnold&#39; e outros fluxos de trabalho não criava nós relevantes no Material Slate Editor, mas abria erroneamente um Maxscript com um erro de compilação. Os nós de fluxos de trabalho, como Arnold, agora são gerados e conectados corretamente de forma automática.
* Resolvido um problema em que exportar ativos/predefinições iniciais (sbsar - mapa de textura Substance2) do Substance 3D Sampler e convertê-los no renderizador Corona (versões 6 a 9hf1) no 3ds Max resultava em materiais corrompidos, renderizando com cor base preta e normais de relevo quebrados. Além disso, essa atualização resolve a inacessibilidade da guia de propriedades do Substance nos materiais, um problema que também afetou as conversões para Vray.
* Correção de um problema no plug-in 3ds Max em que conectar ou desconectar entradas de texturas Substance2 para materiais Corona causava falhas
* Resolvido o problema de compatibilidade no 3ds Max 2024, em que scripts Python incorporados ou chamados em um arquivo MaxScript não eram permitidos por padrão
* Correção de um problema no plug-in 3Ds Max em que a importação e a execução do plug-in Substance para Corona resultavam em materiais pretos e brilhantes em visualizações e renderizações de sombreadores. Esse problema agora foi solucionado com sucesso, garantindo a exibição e a renderização corretas de mapas de Substance com o renderizador Corona.

Esta versão é lançada para o 3ds Max 2021, 2022 e 2023
