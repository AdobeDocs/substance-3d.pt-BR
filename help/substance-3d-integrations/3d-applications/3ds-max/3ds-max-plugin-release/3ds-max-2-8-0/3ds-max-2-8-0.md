---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-2-8-0.html"
breadcrumb-title: ''
description: Consulte as notas de versão do plug-in 3ds Max versão 2.8.0 para saber mais sobre novos recursos, melhorias e correções de erros.
helpx_creative_field: ""
helpx_description: Substance 3D Integrations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max 2.8.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---


# 3ds Max 2.8.0

<b>Adicionado/Atualizado:
</b>

* Suporte para visibilidade condicional de parâmetros (&#39;visible if&#39;); os parâmetros agora ficarão ocultos quando as condições não forem atendidas, com seus respectivos grupos permanecendo visíveis.
* Atualização do renderizador Corona para a versão 10 no plug-in 3ds Max, aprimorando os recursos de renderização e
* A atualização mais recente melhora significativamente a velocidade de renderização e a utilização da CPU no 3ds Max 2024 ao usar o Substance, alinhando seu desempenho mais estreitamente com a eficiência observada no 3ds Max 2022.

<b>Corrigido:</b>

* Melhoria do plug-in Substance para restringir os valores de entrada do teclado dentro do intervalo prático para cada parâmetro, evitando problemas com o controle deslizante e ajustes manuais de valores.
* Correção de um problema em que a cópia de conversões de textura Substance2 (.sbsar) no Slate Material Editor levava a uma instanciação não intencional do nó copiado, potencialmente causando falhas relacionadas ao d3d11.dll
* Correção de um problema de falha no 3ds Max ao renderizar substâncias de material copiadas personalizadas/editadas (.sbsar) com a Corona Interative
* Correção de um problema no nó Substance2 do 3ds Max em que os controles deslizantes para valores inteiros 3 e 4 não respondiam e apenas a entrada numérica manual atualizava os valores. Além disso, esses valores foram exibidos incorretamente no formato flutuante. Os controles deslizantes agora são funcionais e refletem com precisão os tipos de valor desejados.
* Resolvido um problema no 3ds Max 2021 com o Corona Render em que os materiais do Substance apareciam corretamente na viewport, mas eram renderizados em cinza quando os arquivos eram transferidos para outro PC. Os usuários não precisam mais configurar materiais do zero ou carregar predefinições para uma renderização adequada.
* Correção de um problema de falha no plug-in 3ds Max ao tentar duplicar nós Substance no Editor de material de folha.
* Correção de um problema em que a configuração Limite de núcleos de CPU no plug-in Substance não era salva após a reinicialização do 3ds Max, garantindo que os valores configurados pelo usuário agora persistissem entre as sessões.

Esta versão é lançada para o 3ds Max 2021, 2022 e 2023
