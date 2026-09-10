---
helpx_url: "https://helpx.adobe.com/br/substance-3d-bake/guides/performances-and-optimizations.html"
breadcrumb-title: ''
description: Saiba como otimizar a configuração do hardware e a preparação de malha para obter um desempenho de cozimento mais rápido.
helpx_creative_field: ""
helpx_description: bakers > Guides > Performances and optimizations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Desempenho e otimizações
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---


# Desempenho e otimizações

## Requisitos mínimos de hardware

Não há requisitos mínimos para o uso de preparadores de substâncias, no entanto, é importante observar o seguinte:

* Uma boa CPU oferecerá tempos de computação reduzidos (vários núcleos agilizarão o cálculo de **de padeiros de malha** que usam rastreamento de raios).
* Uma quantidade decente de memória (RAM) permitirá carregar malhas com muitos detalhes (polígonos).
* Uma boa GPU permitirá gerar texturas em grandes resoluções (como 8K).

## Triangulação

Os padeiros trabalham internamente com malhas trianguladas; se os modelos 3D (baixo e alto poli) não são triangulados, os padeiros vão triangular as malhas eles mesmos. Esse processo pode ser demorado e aumentará linearmente em relação à quantidade de polígonos contidos no modelo. É geralmente aconselhável triangular as malhas (especialmente a malha alta poli), a fim de evitar que este processo ocorra durante a cozedura.

Se o seu fluxo de trabalho for baseado em FBX, você poderá triangular a malha no momento da exportação usando uma opção no aplicativo DCC.

## Cache de geometria

Consulte a página a seguir para obter mais informações: [Cache de Geometria](../../features/geometry-cache/geometry-cache.md)

## Suavização de borda

Os padeiros podem usar superamostragem para executar suavização de borda. A sobreamostragem significa que os padeiros vão lançar mais raios por pixel, a fim de suavizar o resultado. O tempo de cozedura pode ser drasticamente afetado por essa configuração; isso é particularmente verdadeiro para padeiros onde muitas raias são necessárias, como a oclusão ambiente do padeiro de malha.

Como exemplo:

* um ajuste AA de 2x2 significa que o padeiro lançará 4 vezes a quantidade inicial de raios. Para uma textura de 2048\*2048 px, o cálculo resultante é equivalente a assar uma textura de 4096\*4096px e deve levar cerca de 4 vezes mais tempo para computar.
* uma configuração AA de 8x8 significa que o padeiro vai lançar 64 vezes a quantidade inicial de raios. Para uma textura de 2048\*2048 px, o tempo de computação resultante é equivalente a assar uma textura de 16384\*16384px e deve levar cerca de 64 vezes mais tempo para computar.

**Considerando esses números, a configuração 8x8 deve ser usada com cuidado**.

Para reduzir a presença de ruído, geralmente é aconselhável aumentar o número de raios secundários (para pães normais de oclusão ambiente, thickness e curvatura) e manter uma configuração de AA 2x2 ou 4x4 em vez de usar uma quantidade baixa de raios secundários e uma configuração de AA alta.

>[!NOTE]
>
> Uma boa configuração de desempenho/qualidade para oclusão ambiente da malha é usar AA 2x2 e pelo menos 128 raios secundários.

## Formato de arquivo

A exportação de arquivos em disco pode demorar um tempo significativo, dependendo das configurações de formato de arquivo, resolução, profundidade de bits e compactação. As configurações de compactação podem ser modificadas nas opções Preferências / Projetos / Geral / Formato de arquivo. Desativar a compactação pode diminuir o tempo de exportação em arquivos maiores.

## Falhas e TDR

As falhas podem ser causadas por vários fatores, um deles é o TDR (Timeout Detection Recovery, recuperação de detecção de tempo limite). O TDR é um mecanismo do Windows criado para detectar e se recuperar de situações em que a GPU parece não estar respondendo. Devido a um valor padrão baixo para a detecção de atraso de TDR, podem ocorrer falhas ao usar baker específicos em algumas situações:

* ao fazer bake malhas densas com o baker de Oclusão de ambiente
* ao utilizar os baker acelerados por DXR com malhas muito densas de alto poli (mais de 60 milhões de triângulos)

Você pode encontrar informações adicionais sobre o TDR e um guia passo a passo de como modificar suas configurações associadas aqui: [Os drivers de GPU falham com cálculos longos (falha do TDR)](https://helpx.adobe.com/br/substance-3d/unlisted/documentation/spdoc/gpu-drivers-crash-with-long-computations-128745489.html)
