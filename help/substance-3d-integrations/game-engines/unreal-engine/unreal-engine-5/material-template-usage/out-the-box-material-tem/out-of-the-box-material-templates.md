---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/material-template-usage-ue5/out-of-the-box-material-templates.html"
breadcrumb-title: ''
description: Use modelos de material pré-criados ao importar materiais SBSAR para o Unreal Engine 5 para configuração e fluxos de trabalho rápidos.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 5 > Material Template Usage - UE5 > Out-of-the-Box Material Templates
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Modelos de materiais prontos para uso
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---


# Modelos de materiais prontos para uso

Ao importar materiais do SBSAR para o navegador de conteúdo, você pode escolher os diferentes modelos de material na lista suspensa que estão disponíveis prontos para uso.

![](../../../../../assets/screen-shot-2022-05-10-at-8-58-45-pm-copy.png)

## Modelo Padrão do Substance

Este é um modelo de material básico para uma experiência UV genérica. Ele fornece alguns controles básicos de quantidades UV para que você possa dimensionar os UVs para esticar texturas. É possível dividir a escala UV ativando a opção dividir UV, e você também terá a quantidade U, a quantidade V, o Deslocamento UV e um ângulo de rotação UV. Isso permite que você faça alguns azulejos UV, bem como rotação UV.

![](../../../../../assets/screen-shot-2022-05-10-at-9-06-40-pm-copy.png)

## Modelo Triplanar de Substance

O modelo triplanar faz um mapeamento triplanar dos ângulos X, Y e Z ou faces da malha para que ele mescle três diferentes projeções das texturas para mesclar perfeitamente os ângulos. O modelo triplanar permite que os materiais se misturem entre as faces diferentes à medida que o objeto se dobra

![menu de detalhes para um material Triplanar Substance](../../../../../assets/triplanar-template.png)

O modelo triplanar tem suporte para tamanhos físicos, portanto, quando o tamanho físico está ativado, o modelo triplanar dimensiona as imagens com base no tamanho físico do material. Portanto, não importa o quanto você dimensione seu objeto, essa textura permanecerá sempre a mesma e terá uma aparência uniforme. Saiba mais Tamanho físico aqui: [Tamanho físico - UE5](../../../../../game-engines/unreal-engine/unreal-engine-5/physical-size-ue5/physical-size-ue5.md)

## Modelo de Refração de Substance

O modelo de refração é usado principalmente para objetos transparentes, por exemplo, óculos. Ele permite que você modifique o valor de IOR ou as texturas padrão que teria para um material de vidro ou material transparente.

![](../../../../../assets/screen-shot-2022-05-10-at-9-07-38-pm.png)

## Modelo de pintura de carro Substance

O modelo Pintura de carro adiciona suporte para revestimento claro e inclui suporte para valores e revestimento UV ajustáveis, valores de aspereza de revestimento claro e valores de potência mais frescos.

![menu de detalhes para um material de Pintura de Carro de Substance](../../../../../assets/car-paint-template.png)

## Configurando Modelos de Deslocamento

>[!IMPORTANT]
>
> Modelos Experimentais
> 
> Aviso: os modelos a seguir são experimentais e estão sujeitos a grandes alterações entre as versões. Estes modelos fazem uso da característica Nanite da Epic, que é em si experimental até o momento desta escrita. Elas podem não ser 100% estáveis e deve-se ter cuidado ao usá-las em projetos.

Use as seguintes etapas para habilitar totalmente o suporte a deslocamentos Nanite em seus projetos e usar materiais de deslocamento com suas malhas.

1. Navegue até Pasta do projeto > Config > DefaultEngine.ini e abra-o
1. Anexe o seguinte à seção [/Script/Engine.RendererSettings]:
   * r.Nanite.AllowTessellation=1
   * r.Nanite.Tessellation=1
1. Selecione a malha estática à qual deseja aplicar um modelo de deslocamento e abra suas configurações.
1. Ative a opção Ativar suporte a Nanite.
1. Importe o .sbsar desejado para o navegador de conteúdo e selecione o Substance\_Displacent\_Template ou o Susbtance\_Triplanar\_Displacement\_Template
1. Para alterar a quantidade de deslocamento, navegue até o modelo de material e selecione o nó de saída. Em seguida, ajuste a Magnitude na seção Deslocamento.

## Modelo de Deslocamento Substance

Semelhante ao Modelo padrão de Substance, este modelo permite o ajuste dos valores U e V, adicionando suporte ao Deslocamento Nanite.

![menu de detalhes para um material de Deslocamento do Substance](../../../../../assets/displacement-template.png)

## Modelo de Deslocamento Triplanar Substance

Semelhante ao Modelo de Deslocamento Substance, este modelo aplica-se à projeção triplanar com a opção de suporte a Tamanhos físicos com a adição de suporte a Deslocamentos Nanite.

![menu de detalhes para um material de Deslocamento Triplanar Substance](../../../../../assets/triplanar-displacement-template.png)
