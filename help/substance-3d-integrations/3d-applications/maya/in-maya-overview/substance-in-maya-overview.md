---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/3d-applications/maya/substance-in-maya-overview.html"
breadcrumb-title: ''
description: Saiba mais sobre o plug-in Substance para o Maya e como importar e usar materiais Substance no seu fluxo de trabalho.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Substance in Maya Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Visão geral do Substance no Maya
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---


# Visão geral do Substance no Maya

## Visão geral do plug-in

O plug-in Substance permite carregar um material de Substance criado em Substance Designer diretamente no Maya. O plug-in criará um material do Maya e alimentará as texturas de substância nas entradas de canais de material. Em seguida, você pode fazer alterações nos parâmetros do substance e as texturas serão atualizadas automaticamente.

>[!NOTE]
>
> Verifique se o plug-in está carregado em Configurações/Preferências ->Gerenciador de plug-ins do Maya

![](https://helpx-prod.scene7.com/is/image/HelpxProd/plugin-4?$png$&jpegSize=100&wid=618)

## Abrindo um Substance

1. Abra o Hypershade e, no Editor de nó, clique com o botão direito do mouse e deslize para cima no menu de marcação para escolher criar nó. Isso abre a janela Criar nó. A partir daí, você pode procurar o nó Substance.

   ![](../../../assets/createnode.png)

   Você também pode pressionar Tab no editor de nó e no campo de texto, digite substance e isso filtrará para as opções de substance. Nas opções, escolha Substance Textura.
1. Selecione o nó Substance e no Editor de propriedades e navegue para carregar um arquivo de Substance (.sbsar).

   ![](../../../assets/1.png)
1. A lista suspensa Gráfico selecionado será preenchida se o Substance contiver vários gráficos. O gráfico escolhido será usado para criar o material.
1. O botão Informações do gráfico exibirá os atributos do gráfico definidos no Substance Designer.
1. Defina a Resolução escolhendo um valor na caixa suspensa Largura e Height. A taxa de bloqueio está ativada por padrão.
1. Ative as Saídas de cache para o disco para fazer bake as Saídas de Substance para o disco para que elas possam ser usadas com renderizadores como Arnold. O arquivo armazenado em cache será lido novamente pelo plug-in usando um nó de arquivo do Maya.

   ![](../../../assets/outputsettings.png)
1. Escolha um fluxo de trabalho para o renderizador que você está usando e clique no botão Criar rede de Sombreador. Uma rede de sombreador é criada para o fluxo de trabalho do renderizador. Agora você pode aplicar o material na cena.

   ![](../../../assets/createnetwork.gif){width="1000px"}
