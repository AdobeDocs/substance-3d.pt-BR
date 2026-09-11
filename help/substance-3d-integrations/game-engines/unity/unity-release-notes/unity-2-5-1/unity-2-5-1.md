---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-5-1.html"
breadcrumb-title: ''
description: Consulte as notas de versão do plug-in Unity versão 2.5.1 para saber mais sobre novos recursos, aprimoramentos e correções de erros.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.5.1
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.5.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '246'
ht-degree: 0%

---


# Unity 2.5.1

Lançado em 21 de maio de 2020

Adicionado

* Suporte a Pipeline de Renderização Universal: o Substance textura usará sombreadores e materiais URP automaticamente

Fixa

* Configuração da resolução máxima do mecanismo da CPU Substance:
  * Atualizado o nome do campo no menu Configurações de Substance de “Restrinjo de Textura \*\*” para “Resolução máxima do mecanismo da CPU para Substance”
  * A notificação de aviso será exibida indicando que todos os materiais da substância serão reimportados quando a configuração for modificada
* Removida a mensagem de depuração desnecessária exibida na instalação (”TextureClamp = 4096 Unity.Engine.Debug:Log(Object)”)
* Projeto HDRP: as propriedades de material que estão nos materiais padrão e HDRP continuarão quando os pacotes forem importados e incluírem Substance
* As máscaras Reflexo e HDRP funcionarão conforme o esperado quando um material de Substance de um pacote de Substance que estava na versão anterior do Unity for importado
* Material de Substance duplicado será a cor pretendida e não mais amarelo ao usar a função de duplicação
* A origem do Substance será carregada como esperado após fechar e reabrir o Unity
* Falha ao importar um pacote para um projeto HDRP (intermitentemente)
* O controle deslizante funciona conforme o esperado para materiais de Substance com um parâmetro exposto que tem o Editor definido como Cor (Tons de cinza)
* Falha ao clicar em “Redefinir predefinição como padrão” com gráficos de Substance que não têm resolução padrão
* Falha ao alterar o tamanho de saída de um material de Substance quando o parâmetro de tamanho de saída não é exposto
* A criação do iOS não falhará
* Scripts que usam materiais de Substance serão executados ao criar para Windows Standalone
