---
helpx_url: "https://helpx.adobe.com/br/substance-3d-bake/getting-started/what-is-baking.html"
breadcrumb-title: ''
description: Descubra o que é e saiba como salvar informações de malha 3D em arquivos de textura para aprimorar os materiais em Substance.
helpx_creative_field: ""
helpx_description: "bakers > Getting Started > What is Baking "
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 'O que é cozimento '
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---


# O que é assar?

![](https://upload.wikimedia.org/wikipedia/commons/3/36/Normal_map_example.png)

&#x200B;>> 

(Créditos: [Paolo Cignoni](https://commons.wikimedia.org/wiki/File:Normal_map_example.png) - [CC BY-SA 1.0](https://creativecommons.org/licenses/by-sa/1.0))

Preparação é o nome do processo que envolve **salvar informações** relacionadas a uma **malha 3D** em um arquivo de **textura** ([bitmap](https://en.wikipedia.org/wiki/Raster_graphics)). Na maioria das vezes, esse processo envolve outra malha. Nesse caso, as informações da primeira malha são transferidas para os UVs da segunda malha e, em seguida, salvas em uma textura.

Embora alguns aplicativos possam suportar informações de cozimento nas propriedades de malha (como cores de vértice), os Substance Bakers permitem apenas transformar as informações em uma textura. No entanto, eles podem ler as propriedades de malha e organizá-las em texturas (como cores de vértice).

## Assar é necessário?

O software Substance gera texturas e essas texturas podem ser aprimoradas usando informações relacionadas à geometria da malha.\
Muitos filtros e materiais podem se adaptar à geometria específica de uma malha 3D observando as texturas assadas. A cozedura pode fornecer informações sobre onde as sombras ambientes podem estar, onde estão as bordas da geometria e muito mais.

Por exemplo: um carro antigo pode ter ferrugem aplicada na parte inferior porque ele não se moveu por um tempo. Cozinhar o mapa de posição permitirá saber onde a parte inferior está na malha, o que alimentará o gerador de ferrugem e produzirá a textura adaptada.

![](../../assets/examples.jpg){width="500px"}

## Como funciona a panificação?

Cada padeiro realiza ações específicas a fim de gerar seu próprio resultado, mas em geral o processo de cozedura envolve dois métodos possíveis:

* **Assentar em uma malha** : depende da malha atual para gerar informações.
* **Passando de uma malha para outra**: calcule as informações de uma malha de origem e transfira o resultado para outra.

Esse processo de cozimento depende das propriedades da malha, e é por isso que a malha deve estar limpa e isenta de possíveis falhas em sua geometria.

## Que tipo de informação você pode preparar?

Muitos tipos de informações podem ser analisadas. No entanto, em geral, apenas um conjunto específico é necessário porque eles podem ser extrapolados para criar resultados mais avançados posteriormente. É por isso que existem tipos comuns de processo de cozimento que podem ser encontrados em vários softwares.

Como exemplo, o software de Substance pode gerar o seguinte tipo de informação:

* **oclusão de ambiente** (sombras de ambiente)
* Informações **Normais** (variações de detalhes da superfície armazenadas como direções de vetor)
* **Direção** (onde é para cima ou para baixo, esquerda ou direita etc.)
* **Curvatura** (bordas e cavidades da geometria)
* **Posição** (posição relativa da geometria dentro de um cubo normalizado)

Consulte a [documentação de cada padeiro](../../bakers-settings/bakers-settings.md) para obter mais informações.

## Diferença entre padarias &#39;regulares&#39; e &#39;de malha&#39;

Dependendo do processo, os padeiros usam várias implementações. De modo geral, os **padeiros de malha** contam com técnicas de traçado de raio para extrair e projetar dados de um modelo para outro.
