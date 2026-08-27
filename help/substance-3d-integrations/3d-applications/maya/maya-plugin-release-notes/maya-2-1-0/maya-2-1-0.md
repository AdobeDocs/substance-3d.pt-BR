---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/maya/maya-plugin-release-notes/maya-2-1-0.html"
breadcrumb-title: ''
description: Consulte as notas de versão do plug-in Maya versão 2.1.0 para saber mais sobre novos recursos, aprimoramentos e correções de erros.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Maya Plugin Release Notes > Maya 2.1.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Maya 2.1.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '357'
ht-degree: 0%

---


# Maya 2.1.0

Substance no Maya 2.1.0 changelog

* Compatibilidade garantida com o Python 3
* Substance Engine atualizado para a versão 7.2.9
* Correção de um erro com nomes de variáveis mel globais conflitantes ao aplicar um fluxo de trabalho
* O fluxo de trabalho do Redshift agora define o fresnel como metalness
* Adicionado novo arquivo de plug-in, substancelink, que lida com a interoperabilidade com outros programas Substance e o Substance Launcher
* Ao abrir o Substance Source agora, o Iniciador de Substance será aberto na guia Código-fonte se o plug-in substancelink estiver carregado
* O plug-in substancelink permite que o Iniciador, quando a interface do usuário é adicionada, envie materiais de Substance Source para a integração do Maya
* Comandos de script adicionados para obter versões internas da biblioteca, bem como para abrir o Substance Launcher na página de origem
* Links de sites agora abertos para [substance3d.com](http://substance3d.com) em vez de [allegorithmic.com](http://allegorithmic.com)
* A documentação e os links de origem, ao abrir uma página da Web, agora abrirão o navegador padrão definido pelo usuário
* No Windows, o Internet Explorer não está mais aberto
* Adicionado novo link na prateleira e menu ao Substance share
* Adicionados novos comandos para consultar a versão e o hash do Vinculador de Substance
* No Maya LT, a versão foi removida do menu de configurações
* O menu Sobre não está mais escrito em PySide2 e Python, mas em código nativo usando Qt. Está agora disponível no Maya LT, onde anteriormente não estava.
* O menu Sobre tem informações de diagnóstico diferentes; ele agora exibe o hash git para corresponder à alteração no controle do código-fonte
* A cópia do menu Sobre para a área de transferência agora também terá este hash git, juntamente com a versão do Maya para a qual o plug-in foi criado.
* As licenças na janela Sobre agora abrem como um arquivo de texto
* Suporte adicionado ao Maya 2017
* O gerador de script de fluxo de trabalho não gera mais cadeias de caracteres para o membro &#39;ordenação&#39;. Todos os fluxos de trabalho existentes serão tratados adequadamente

Comandos de script adicionados:\
Substância:\
\* substanceUtilityGetLinkerVersion\
\* substanceUtilityGetLinkerHash\
\* substanceUiOpenAboutWindow\
\* substanceUiOpenSourceWebsite\
\* substanceUiOpenDocumentation\
\* substanceUiOpenShareWebsite

substancelink:\
\* substanceLinkGetLinkVersion\
\* substanceLinkGetPortalCliVersion\
\* substanceLinkOpenLauncher

Esta versão é lançada para o Maya 2017, 2018, 2019 e 2020 no Windows,\
Linux e Macos. Também foi lançado para o Maya LT 2018, 2019 e 2020 em\
Windows e MacOS.
