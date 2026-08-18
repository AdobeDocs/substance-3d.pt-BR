---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/3d-applications/cinema-4d/attribute-manager.html"
breadcrumb-title: ''
description: Use o Gerenciador de atributos do Cinema 4D para definir as propriedades de ativos de Substance e as configurações de materiais.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Cinema 4D > Attribute Manager
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Gerenciador de Atributos
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---


# Gerenciador de Atributos

Há um novo modo para os ativos de Substance no Gerenciador de atributos do Cinema 4D.

Quando um Substance é selecionado no Gerenciador de ativos do Substance, o Gerenciador de atributos alternará automaticamente para o modo de ativos de Substance. Você também pode alternar manualmente para esse modo no menu do modo do Gerenciador de atributos.

No modo de ativo de Substance, você tem acesso a todas as entradas de um Substance e também tem uma visão geral de todos os canais de saída.

![](../../../assets/cinema-4d-9.png){width="500px"}

## Agrupamento de Entradas de Substance

Se as entradas de um Substance forem agrupadas, esses grupos serão mostrados como tal no Gerenciador de atributos. Há dois grupos predefinidos: **Propriedades básicas** e **Entradas de imagem**.

* No grupo Propriedades básicas, todas as entradas que não foram atribuídas a um grupo no Substance Designer serão exibidas.
* Como o nome já sugere, todas as Entradas de Substance vinculadas a imagens externas são coletadas no grupo Entradas de imagem.

## Parâmetro de nome de arquivo

Ao usar o parâmetro Nome do arquivo no Gerenciador de atributos, o local do arquivo dos ativos de Substance pode ser alterado depois que eles são carregados em uma cena.

![](../../../assets/cinema-4d-10.png){width="500px"}

Isso pode ser útil não apenas para realocar arquivos de Substance, mas também ao trocar um Substance com um completamente diferente.

Nesse caso, o usuário será perguntado se alguma referência existente a canais de saída de Substance anteriores deve ser remapeada para o novo Substance.

![](../../../assets/cinema-4d-11.png){width="500px"}

Se a pergunta for respondida com &#39;Não&#39;, os links para o Substance anterior serão excluídos de todos os sombreadores de Substance. Para remapear os canais de saída, o plug-in primeiro procurará canais de saída com o mesmo tipo e, em seguida, com o mesmo nome.

## Triestado do Parâmetro

Se vários Substance forem selecionados ao mesmo tempo, as entradas compartilhadas entre esses Substance serão mostradas como de três estados e podem ser editadas para todos os Substance selecionados simultaneamente (assim como todos os outros parâmetros no Cinema 4D).

Nesses casos, os canais de saída serão exibidos conforme mostrado abaixo.

![](../../../assets/cinema-4d-12.png){width="300px"}
