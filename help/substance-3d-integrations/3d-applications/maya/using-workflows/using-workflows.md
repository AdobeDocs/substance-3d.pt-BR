---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/3d-applications/maya/using-workflows.html"
breadcrumb-title: ''
description: Crie e use predefinições de renderização para saídas de Substance no Maya para gerar automaticamente redes de sombreador para renderizadores diferentes.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Using Workflows
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Uso de fluxos de trabalho
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---


# Uso de fluxos de trabalho

Em Fluxos de trabalho, você pode escolher ou criar predefinições de renderização para saídas de Substance. Essas predefinições são redes de sombreador para um renderizador como Arnold ou Vray.

>[!NOTE]
>
> **Locais Predefinidos de Fluxo de Trabalho**
> 
> **Windows**:\
> C:\Users\\Documents\maya\2022\substance\workflows\generated\
> **MacOS**:\
> /Users//Library/Preferences/Autodesk/maya//substance/workflows/generated\
> **Linux**:\
> /home//maya//substance/workflows/generated

![](../../../assets/workflows-4.png)

Para usar um fluxo de trabalho, basta escolher a predefinição na lista suspensa e, em seguida, clicar no botão Criar rede de Sombreador.

![](../../../assets/workflow.gif)

## Criando um Fluxo de Trabalho

Você pode criar seu próprio fluxo de trabalho e adicioná-lo à lista Fluxo de trabalho do renderizador. Ao adicionar um novo fluxo de trabalho, todos os nós criados após o nó Substance serão salvos no fluxo de trabalho. Isso permite que você crie qualquer número de nós de sombreamento para criar uma rede de sombreador personalizada completa que pode ser salva como um fluxo de trabalho predefinido.

## ![](../../../assets/saved-workflow.png) Gerenciamento de Fluxos de Trabalho

### Salvar fluxos de trabalho personalizados

1. Crie manualmente saídas de Substance e conecte-as a um material como aiStandardSurface.
   1. Você pode usar qualquer Maya ou nós específicos de renderização para criar a rede de sombreador.
1. Clique no botão **Criar Fluxo de Trabalho** e insira um nome para a predefinição de fluxo de trabalho.

### Duplicação de fluxos de trabalho

Você pode duplicar um fluxo de trabalho clicando no botão **Duplicar Fluxo de Trabalho**.

### Renomear e substituir fluxos de trabalho

Você pode renomear fluxos de trabalho existentes e substituir fluxos de trabalho por dados atualizados usando os botões selecionados **Renomear** e **Substituir**.

### Removendo fluxos de trabalho

É possível remover fluxos de trabalho existentes usando o botão Remover fluxo de trabalho.
