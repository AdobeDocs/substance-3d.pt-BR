---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-4-5.html"
breadcrumb-title: ''
description: Consulte as notas de versão do plug-in Unity versão 2.4.5 para saber mais sobre novos recursos, aprimoramentos e correções de erros.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.4.5
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.4.5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---


# Unity 2.4.5

Lançado em 6 de abril de 2020

* Adicionado: Verificação de ativos HDRP usando a API 2019.3
* Adicionado: atualização do Substance Engine 7.2 - corrige alguns materiais do Substance de origem não funcionam
* Adicionado: Atualize as configurações de destino para corresponder à resolução da CPU
* Adicionado: configuração de resolução máxima do mecanismo da CPU (configuração de 4k ou 2k)
* Adicionado: Converter Substance(s) não HDRP em um projeto HDRP
* Correção: falha ao importar grande quantidade de Substance
* Correção: exceção ao clicar em reimportar no modo de reprodução após alterar os parâmetros Substance
* Corrigido: valide a resolução (textura) de saída (API para limitar o mecanismo da CPU a 2K) preferência do usuário para definir o padrão para 4K
* Correção: clicar em “Gerar mapas de mixagem” em um gráfico de Substance no modo de reprodução resulta em um travamento infinito
* Correção: ao usar o plug-in Substance em um projeto HDRP, o uso da compactação Raw define as texturas em tons de cinza como Alpha
* Corrigido: GameObject desmarcado no modo de reprodução
* Corrigido: o mapa de aspereza não está sendo atualizado com a alteração do parâmetro
* Correção: a saída da máscara não é gerada corretamente para alguns arquivos Substance em HDRP
* Correção: falha ao alternar o menu suspenso de mapa alfa compactado entre duas opções
* Correção: a caixa de seleção Instância de GPU é revertida ao clicar fora do material do Substance.
* Correção: ao usar a função Duplicate(), o gráfico de Substance duplicado não tem o smoothness compactado no alfa do metálico corretamente.
* Correção: alternar o destino de compilação para o Android resulta no formato incorreto das texturas até que sejam reimportadas manualmente.
* Corrigido: excluir um arquivo de Substance no Unity causará uma NullReferenceException.
* Corrigido: desabilitar o uso da API HDRP do Unity 2019.3 para versões anteriores

Problemas conhecidos:

* A caixa de seleção de emissão não é ativada por padrão e o valor HDR é definido como preto na importação de um Substance.
* As propriedades dos materiais de embalagens com materiais de substância padrão não são mantidas na importação.
* A atualização de 2017-2019/2020 não funciona no HDRP
* Clicar na opção de fixação 2048 no menu de configurações enquanto seleciona 4096 nas configurações de destino (sem clicar em aplicar) resulta em um erro no registro do console
