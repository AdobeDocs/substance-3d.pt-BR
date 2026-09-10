---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/game-engines/unity/generated-textures-packing.html"
breadcrumb-title: ''
description: Entenda como o Substance gera texturas no Unity e configure a embalagem de textura para entradas de sombreador ideais.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Generated Textures (Packing)
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Texturas geradas (Embalagem)
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 6%

---


# Texturas geradas (Embalagem)

As Textura geradas mostram as saídas do Substance que são computadas pelo Substance Engine para criar texturas. Essas texturas são alimentadas nas entradas de sombreador. Por padrão, apenas as entradas base usadas pelo sombreador são criadas. Se a opção “Gerar todas as saídas” estiver ativada, todas as texturas serão exibidas aqui.

![](../../../assets/screen-shot-2022-03-29-at-1-24-16-pm-copy.png)

Quando a opção “Gerar todas as saídas” estiver ativada

![](../../../assets/screen-shot-2022-03-29-at-1-29-35-pm-copy.png)

## Uso

1. Selecionar um ícone de textura selecionará a textura na janela Projeto. Isso não funciona para materiais em tempo de execução porque as texturas não são geradas na pasta do projeto.
1. O botão sRGB funciona de forma semelhante à opção sRGB (textura de cores) nas Configurações de importação de Textura. Permite definir se uma textura deve ser interpretada em espaço gama (sRGB) ou linear. O plug-in Substance lida com essa interpretação automaticamente, mas pode ser substituído se necessário.

   | Saída de Substance | sRGB |
   | --- | --- |
   | Cor de base | Ativada |
   | Difusão | Ativada |
   | Especular | Ativada |
   | Normal | Desativado |
   | Metálico | Desativado |
   | Rugosidade | Desativado |
   | Textura reluzente | Desativado |
   | Altura | Desativado |
   | Oclusão de ambiente | Desativado |

## Embalagem canais

É possível empacotar uma textura no canal alfa de outra textura usando o menu suspenso. Cada textura gerada tem um menu suspenso que contém uma lista de todas as saídas de textura geradas pelos materiais de Substance. Basta escolher um mapa da lista para embalá-lo no canal alfa da textura. A opção Origem é o canal alfa da textura.

Nesta imagem, selecionei o mapa de altura:

![](../../../assets/screen-shot-2022-03-29-at-2-48-33-pm.png)

Na imagem a seguir, você pode ver que a saída do height está sendo empacotada no canal alfa do mapa de cor de base.

![](https://helpx-prod.scene7.com/is/image/HelpxProd/screen-shot-2022-03-29-at-2-53-20-pm-copy?$png$&jpegSize=200&wid=1248)

## Mapeamento da Textura de saída

Além disso, a textura de saída pode ser atribuída individualmente às Entradas de superfície de materiais do Unity por meio da seção Mapeamento de Textura de saída. As texturas de saída geradas pelo .sbsar serão exibidas na coluna esquerda, e as Entradas de superfície da unidade disponíveis aparecerão na coluna direita. A última opção pode ser alterada nos menus suspensos.

![](../../../assets/image2023-3-27-14-30-24.png)
