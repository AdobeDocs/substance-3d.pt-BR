---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/3d-applications/blender/the-substance-3d-panel.html"
breadcrumb-title: ''
description: Saiba como usar o painel Substance 3D no Blender para gerenciar materiais, parâmetros e saídas.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > The Substance 3D Panel
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: O painel Substance 3D
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---


# O painel Substance 3D

![](../../../assets/blender-substance3dpanel.png)

## Controles do painel

**Criar** - Abre o navegador de arquivos para selecionar um material do Substance 3D. Por padrão, isso cria um material de mesclagem usando texturas geradas a partir do arquivo .sbsar.

**Aplicar** - Anexe o material selecionado do Substance 3D aos objetos selecionados em um novo slot de material. Isso não substitui as atribuições de material anteriores no objeto.

**Ativos da comunidade do Substance 3D** - abre a página Ativos da comunidade do Substance 3D no navegador da Web.

**Substance 3D Assets** - Abre a página de origem do Substance 3D Assets no navegador da Web.

**Duplicar material selecionado do Substance 3D** - Carregue uma nova instância do material selecionado do Substance 3D. Os parâmetros de diferentes instâncias do mesmo material de Substance podem ser ajustados independentemente um do outro.

**Atualizar** - Recarrega o material do Substance 3D

>[!WARNING]
>
> **Aviso:**
> 
> O uso do botão atualizar desfará todas as alterações do usuário no gráfico de sombreador. Copie todos os nós adicionados pelo usuário antes de atualizar para colá-los no gráfico após a atualização.

**Remover** - Remove o material do Substance 3D selecionado do painel.

>[!NOTE]
>
> O material do Blender criado a partir do material de Substance permanecerá no projeto. Ela pode ser excluída ou removida dos objetos manualmente.

**Materiais de Substance 3D carregados** - Exibe uma lista dos Materiais de Substance que foram carregados no arquivo .blend.

## Parâmetros de gráfico

**Resolução de saída** - listas suspensas para a resolução with e height. Eles podem ser desvinculados para ajustar os valores de forma independente.

**Aleatório e Distribuição Aleatória** - O botão aleatório gera um novo valor de distribuição aleatória para alterar parâmetros que podem usar valores aleatórios. A semente aleatória também pode ser definida manualmente.

## Trabalhar com predefinições

Os arquivos SBSAR podem ser publicados com predefinições, que podem ser encontradas na caixa suspensa Predefinições. Para criar suas próprias predefinições, ajuste os parâmetros conforme desejado e use o botão **Salvar**. Há opções adicionais para exportar a predefinição selecionada como um arquivo .sbsprs e para excluir a predefinição selecionada da lista suspensa. O botão **Carregar** pode ser usado para importar predefinições de arquivos .sbsprs.

## Parâmetros Substance

Os parâmetros que foram expostos no Substance Designer podem ser ajustados usando os controles de parâmetro do Substance. Esses parâmetros são definidos pelo criador do Material de Substance e variam entre os materiais. Ajustar esses parâmetros atualizará as texturas geradas, conforme indicado pelo ícone de processamento ao lado do nome do material na seção Materiais de Substance 3D carregados.

O formato de arquivo das texturas de saída pode ser alternado e alterado nos menus suspensos.

Para obter mais informações, consulte [Expondo um parâmetro](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/substance-graphs/manage-parameters/exposing-a-parameter) na página de documentação do Designer.

## Parâmetros técnicos

Os materiais Substance podem ter um conjunto de parâmetros técnicos. Esses são controles adicionais para correção de cores e outros ajustes de material.
