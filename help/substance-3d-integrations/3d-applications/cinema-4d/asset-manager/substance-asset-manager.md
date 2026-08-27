---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/cinema-4d/substance-asset-manager.html"
breadcrumb-title: ''
description: Use o Substance Asset Manager no Cinema 4D para adicionar, remover e organizar materiais Substance na cena.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Cinema 4D > Substance Asset Manager
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance Asset Manager
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 0%

---


# Substance Asset Manager

A janela do Substance Asset Manager lista todos os Substance carregados em uma cena. Aqui você pode adicionar, remover e reorganizar Substance.

Selecionar (clique com o botão esquerdo) um Substance dentro do Substance Asset Manager abre o Substance no Attribute Manager do Cinema 4D. Lá, você pode alterar os parâmetros e as entradas de Substance de quadro-chave como qualquer outro parâmetro no Cinema 4D.

>[!NOTE]
>
> O Gerenciador de atributos tem um modo de ativo de Substance especial, que é útil para ter um Gerenciador de atributos dedicado para Substance no seu layout de Cinema 4D.

![](../../../assets/cinema-4d-4.png){width="500px"}

## Menu Arquivo

## Carregar ativo...

Carregue um novo Substance na cena (o mesmo que no menu Plug-ins).

Fechar

Fecha o Substance Asset Manager. Os Substance carregados, é claro, ficarão na cena.

## Menu Editar

## Selecionar todos os Substance

Seleciona todos os Substance listados no Gerenciador de ativos. O mesmo pode ser obtido pressionando Ctrl+a, enquanto o mouse passa sobre o Gerenciador de ativos.

## Desmarcar todos os Substance

Desmarca todos os Substance listados no Gerenciador de ativos. O mesmo pode ser obtido pressionando Shift+Ctrl+a, enquanto o mouse passa sobre o Gerenciador de ativos.

## Selecionar de Material(is) Selecionado(s)

Seleciona todos os Substance referenciados pelos *materiais* selecionados no momento.

## Selecionar material(is) marcado(s)

Seleciona todos os Substance referenciados pelos materiais *marcados* atualmente. No Cinema 4D, um material é marcado se um objeto ou tag que usa esse material for selecionado.

## Selecionar material(is)

Seleciona todos os materiais que fazem referência aos Substance selecionados atualmente.

## Menu Ações

## Criar material(is)

Criar novos materiais a partir dos Substance selecionados atualmente. Os canais de material serão inicializados automaticamente com sombreadores de Substance referentes aos respectivos canais de saída dos Substance.

## Duplicar Substance(s)

Duplica os Substance selecionados atualmente. Isso pode ser útil para usar o mesmo Substance com diferentes conjuntos de parâmetros em vários materiais.

## Reimportar Substance(is)

Esta função pode ser usada para retornar aos valores padrão de um Substance ou para integrar alterações externas (por exemplo, do Substance Designer).\
Observação: **Todas as** alterações de parâmetro nas entradas de Substance serão perdidas!

## Remover Substance(s)

Remove os Substance selecionados atualmente da cena. O mesmo pode ser feito pressionando a tecla Delete enquanto o mouse passa por cima do Gerenciador de ativos.

## Excluir Substance(s) não utilizado(s)

Remove todos os Substance atualmente não referenciados por nenhum material.

## menu Substance Engine

O conteúdo desse menu depende do sistema operacional no qual o Cinema 4D está sendo executado. A alteração do Substance Engine só terá efeito após uma reinicialização do Cinema 4D.

## Menu de contexto

Ao clicar com o botão direito do mouse em um Substance selecionado, o menu de contexto será exibido. Sua funcionalidade é a mesma das funções com nomes idênticos nos menus acima mencionados:

* Remover
* Criar material(is)
* Duplicar Substance
* Reimportar Substance
* Selecionar todos os Substance
* Desmarcar todos os Substance
* Selecionar material(is)

## Arrastar e soltar

Você pode interagir com o Substance Asset Manager arrastando e soltando. Há várias opções disponíveis:

* Carregue Substance(s) na cena arrastando e soltando do Explorer ou do Finder, simplesmente soltando-os no Gerenciador de ativos do Substance.
* Substance pode ser arrastado para o campo de vínculo de sombreadores de Substance para conectar um sombreador e um ativo de Substance.
* Se estiver no modo Não classificado (veja abaixo), você pode reorganizar Substance no Gerenciador de ativos arrastando-os para um novo local.


## Classificação no Substance Asset Manager

## Modo não classificado

## O Substance Asset Manager está no **Modo não classificado por padrão**. A célula de cabeçalho da coluna de nome não exibe uma seta à direita. Você pode usar arrastar e soltar para reorganizar as substâncias como desejar.

![](../../../assets/cinema-4d-3.png){width="500px"}

![](../../../assets/cinema-4d-5.png){width="500px"}

## Visualizações no Substance Asset Manager

## O Substance Asset Manager exibe ícones pequenos com visualizações dos canais disponíveis para cada Substance.

## As visualizações são simplesmente exibidas na ordem dos canais de saída no Substance. A coluna na qual a visualização é exibida não tem nenhum significado.
