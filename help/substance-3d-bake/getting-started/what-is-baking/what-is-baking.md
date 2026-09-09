---
helpx_url: 'https://helpx.adobe.com/br/substance-3d-bake/getting-started/what-is-baking.html'
breadcrumb-title: ''
description: Descubra o que é fazer bake e saiba como salvar informações de malha 3D em arquivos de textura para aprimorar os materiais em Substance.
helpx_creative_field: ''
helpx_description: 'bakers > Getting Started > What is Baking '
helpx_experience_level: ''
helpx_learn_topic: ''
helpx_tags: ''
title: 'O que está Fazendo bake '
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0a948aa65b787c0f84e0af681dbe74021e878687
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---


# O que é Fazer bake?

![](https://upload.wikimedia.org/wikipedia/commons/3/36/Normal_map_example.png)

(Créditos: [Paolo Cignoni](https://commons.wikimedia.org/wiki/File:Normal_map_example.png) - [CC BY-SA 1.0](https://creativecommons.org/licenses/by-sa/1.0))

Preparação é o nome do processo que envolve **salvar informações** relacionadas a uma **malha 3D** em um arquivo de **textura** ([bitmap](https://en.wikipedia.org/wiki/Raster_graphics)). Na maioria das vezes, esse processo envolve outra malha. Nesse caso, as informações da primeira malha são transferidas para os UVs da segunda malha e, em seguida, salvas em uma textura.

Embora alguns aplicativos possam oferecer suporte à faz bake de informações nas propriedades de malha (como cores de vértice), os Substance Bakers permitem apenas fazer bake informações em uma textura. No entanto, eles podem ler as propriedades de malha e organizá-las em texturas (como cores de vértice).

## Fazer bake é necessário?

O software Substance gera texturas e essas texturas podem ser melhoradas usando informações relacionadas à geometria da malha.\
Muitos filtros e materiais podem se adaptar à geometria específica de uma malha 3D observando as texturas feitas bake. O fça bake pode fornecer informações sobre onde podem estar as sombras ambientes, onde estão as bordas da geometria e muito mais.

Por exemplo: um carro antigo pode ter ferrugem aplicada na parte inferior porque ele não se moveu por um tempo. Fazer bake o mapa de posição permitirá saber onde a parte inferior está na malha que alimentará o gerador de ferrugem e produzirá a textura adaptada.

![](../../assets/examples.jpg){width="500px"}

## Como funciona o faço bake?

Cada baker executa ações específicas a fim de gerar seu próprio resultado, mas em geral o processo de fça bake envolve dois métodos possíveis:

* **Fazendo bake em uma malha** : depende da malha atual para gerar informações.
* **Fazendo bake de uma malha para outra**: calcule as informações de uma malha de origem e transfira o resultado para outra.

Esse processo de fça bake depende das propriedades da malha, e é por isso que a malha deve estar limpa e isenta de possíveis falhas em sua geometria.

## Que tipo de informação você pode fazer bake?

Muitos tipos de informações podem ser feitos bake. No entanto, em geral, apenas um conjunto específico é necessário porque eles podem ser extrapolados para criar resultados mais avançados posteriormente. É por isso que existem tipos comuns de processo de faço bake que podem ser encontrados em vários softwares.

Como exemplo, o software de Substance pode gerar o seguinte tipo de informação:

* **Oclusão de ambiente** (sombras ambientes)
* Informações **Normais** (variações de detalhes da superfície armazenadas como direções de vetor)
* **Direção** (onde é para cima ou para baixo, esquerda ou direita etc.)
* **Curvatura** (bordas e cavidades da geometria)
* **Posição** (posição relativa da geometria dentro de um cubo normalizado)

Consulte a [documentação de cada baker](../../bakers-settings/bakers-settings.md) para obter mais informações.

## Diferença entre Baker &#39;regular&#39; e &#39;de malha&#39;

Dependendo do processo, os baker usam várias implementações. Em geral, os baker **de malha** contam com técnicas de Rastreamento de raios para extrair e projetar dados de um modelo para outro.
