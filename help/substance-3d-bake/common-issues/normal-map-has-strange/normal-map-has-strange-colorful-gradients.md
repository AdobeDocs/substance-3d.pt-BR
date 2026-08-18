---
helpx_url: "https://helpx.adobe.com/br/substance-3d-bake/common-issues/normal-map-has-strange-colorful-gradients.html"
breadcrumb-title: ''
description: Corrija gradientes coloridos estranhos em mapas normais, verificando normais de malha, grupos de suavização e mapeamento UV.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Normal map has strange colorful gradients
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: O mapa normal tem gradientes coloridos estranhos
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---


# O mapa normal tem gradientes coloridos estranhos

A saída do padeiro é um conjunto de gradientes coloridos muito fortes.

![](../../assets/color-gradient.png)


## Explicação

Gradientes coloridos geralmente acontecem quando há uma incompatibilidade entre a malha de alto e baixo polígono durante o processo de cozimento. Esta incompatibilidade pode ser explicada pelo seguinte motivo:

* A malha de alto e baixo polígono <b>não se sobrepõe</b> corretamente (veja a imagem abaixo).
* O alto-polivalente é a <b>geometria ausente</b> que o baixo-polivalente tenta cobrir.
* A malha de alto ou baixo-poli tem normais de vértice invertidos.

Quando acontece, o processo de cozimento tenta combinar com uma geometria que não existe, resultando em algo vazio. O padeiro preenche essa área vazia com uma cor extraída dos pixels vizinhos nas texturas, criando o degradê colorido (a menos que a <b>Difusão</b> esteja desabilitada).

## Solução

Dadas as poucas razões possíveis que levam à não sobreposição das malhas, há que considerar algumas soluções:

* Certifique-se de congelar/redefinir a transformação de malha (redefinir forma x etc.) para ter certeza de que todas as malhas são consistentes
* Importe as malhas de baixo e alto nível no software de modelagem 3D para verificar se elas se sobrepõem corretamente
* Certifique-se de que sua convenção de nomenclatura seja válida se você estiver usando o recurso [Correspondência por Nome](../../features/matching-by-name/matching-by-name.md) (você pode verificá-la cozinhando e, em seguida, examinando o arquivo de log que deve imprimir os nomes de malha).

### Exemplo

Abaixo está um exemplo com uma esfera de alto-poli e baixo-poli. À esquerda, as malhas não se sobrepõem porque o alto-polietileno foi deslocado para fora :

![](../../assets/baking-gradients.jpg)
