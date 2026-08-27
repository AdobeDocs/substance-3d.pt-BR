---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/3d-applications/modo/substance-in-modo-overview.html"
breadcrumb-title: ''
description: Saiba mais sobre o plug-in Substance para MODO e como importar e usar materiais Substance no seu fluxo de trabalho.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Substance in MODO Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance na visão geral do MODO
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 5%

---


# Substance na visão geral do MODO

## Visão geral:

## Abrindo um Substance

1. Crie um material ou selecione um grupo de materiais.
1. Em Textura>Substance, escolha criar Substance ou use o botão Criar nas opções do Kit de Substance. Isso criará um material de Substance na árvore sombreadora.
1. Clique em Carregar sbsar para carregar um arquivo sbsar.

   ![](../../../assets/load-1.png)

## Criando Saídas

Usando o **Padrão - Modo de Sombreamento de Princípios**, você pode criar saídas usando o fluxo de trabalho metálico/rugosidade.

1. Na seção Saídas das Propriedades do Substance, clique nas saídas necessárias para o sombreamento. A textura do Substance será gerada, adicionada à Árvore sombreadora com o efeito de camada de material correto. Para o Modo de Sombreamento de princípios, você precisará do seguinte:

   | Saída de Substance | Espaço de cores | Efeito de camada de material (modo de Sombreamento de princípios) |
   | --- | --- | --- |
   | Cor de base | sRGB | Cor difusa |
   | Normal | Linear | Normal |
   | Rugosidade | Linear | Rugosidade |
   | Metálico | Linear | Metálico |

   ![](../../../assets/outputs-3.png)

## Alteração de Resolução/Parâmetros

Você pode alterar os parâmetros de Substance para atualizar ou alterar as texturas geradas. Alterar um parâmetro fará com que o Substance Engine recalcule as texturas que são alimentadas no material MODO.

1. Vá para as Propriedades de Substance do material de Substance e, na seção Ajustes, altere qualquer um dos parâmetros.

   ![](../../../assets/params.png)
1. Você pode alterar a resolução das texturas geradas usando o menu suspenso Tamanho da saída. Os Substance podem ser configurados para gerar até 8K. O [mecanismo GPU de Substance](../../../3d-applications/modo/modo-switch-engine/modo-switch-engine.md) é necessário para a saída 8K.
