---
helpx_url: "https://helpx.adobe.com/br/substance-3d-bake/getting-started/software-interface/substance-3d-designer.html"
breadcrumb-title: ''
description: Saiba como acessar e usar a janela de cozimento no Substance 3D Designer para transformar informações de modelo em texturas.
helpx_creative_field: ""
helpx_description: bakers > Getting Started > Software Interface > Substance 3D Designer
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance 3D Designer
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 2%

---


# Substance 3D Designer

![](../../../assets/sd-mesh-right-click.png)

A janela de cozimento pode ser acessada por meio do arquivo de malha na janela do [Explorer](https://helpx.adobe.com/br/substance-3d/unlisted/documentation/sddoc/the-explorer-129368147.html). Clique com o botão direito do mouse no nome da malha e escolha “**Informações do modelo de cozimento**” para abrir a janela de cozimento.

## Visão geral

![](../../../assets/sd-window-overview.png){width="500px"}

A janela de cozedura de é dividida em vários painéis que são descritos abaixo.

### Elemento para assar

![](../../../assets/sd-mesh-selection.png)

Este painel controla qual parte da malha de baixo-poli será usada para realizar a cozedura.

Esse painel listará a geometria encontrada dentro do arquivo de malha de baixo polígono. Por padrão, a lista é baseada nos materiais individuais encontrados no arquivo, mas pode ser alterada para submalhas quando relevante. Você pode desmarcar os elementos que devem ser ignorados durante o processo de cozimento.

### Saída

![](../../../assets/sd-output.png)

Esse painel controla onde a textura assada será localizada.

| *Parâmetro* | *Descrição* |
| --- | --- |
| **Método** | Controla como as texturas assadas serão armazenadas com o pacote de Substance.Valores possíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Incorporada</strong>: a textura cozida é armazenada em uma subpasta próxima ao pacote de Substance com nome específico.</li><li data-preserve-html="true"><strong>Vinculado</strong> (padrão): a textura cozida é armazenada na pasta definida e referenciada no Substance empacotado.</li></ul> |
| **Pasta** | Local das texturas assadas quando salvas. Clique no botão de três pontos para abrir uma caixa de diálogo de arquivo e escolher a pasta de exportação. Uma marca de seleção estará visível à direita para indicar se a pasta realmente existe ou não. |
| **Nome** | Convenção de nomenclatura das texturas assadas. Clique no botão de três pontos para abrir um menu suspenso e inserir outros espaços reservados (nome do banco, personalizado, material, malha). |
| **Amostra** | Simule um nome de arquivo para testar a convenção de nomenclatura. |
| **Colocar Recurso em uma Pasta Específica do Mesh** | Se ativadas, as texturas cozidas serão salvas dentro de uma pasta nomeada como arquivo de malha. |

### Malhas de alta definição

![](../../../assets/sd-high.png)

Este painel controla a lista de malha de alto polígono e as configurações relacionadas. Consulte os [parâmetros comuns](../../../bakers-settings/common-parameters/common-parameters.md) para obter mais informações.

### Valores padrão

![](../../../assets/sd-default-values.png)

Consulte os [parâmetros comuns](../../../bakers-settings/common-parameters/common-parameters.md) para obter mais informações.

### Lista e configurações de Baker

![](../../../assets/sd-baker-list.png)

É no padeiro que você pode escolher qual textura assada deseja gerar. Por padrão, a lista está vazia.

* **Adicionando um novo padeiro:** Clique no botão “Adicionar Padeiro”.
* **Remoção de um padeiro:** selecione o padeiro na lista e, em seguida, clique no botão “Excluir o padeiro”.
* **Movendo um padeiro para o topo:** selecione o padeiro na lista e clique no botão “Puxar para o topo”.
* **Movendo para baixo um padeiro:**&#x200B;Selecione o padeiro na lista, em seguida, clique no botão “Empurrar para baixo”.

Cada padeiro no herda por padrão os Valores padrão (veja acima). O tamanho (resolução), por exemplo, pode ser substituído clicando na célula na linha do padeiro. Isso é verdadeiro para as outras configurações na linha.

Ao clicar em um padeiro na lista, a visualização Parâmetros Baker atualizará com seus parâmetros específicos.

Para saber mais sobre os parâmetros específicos, consulte: [Configurações de preparadores](../../../bakers-settings/bakers-settings.md).
