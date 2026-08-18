---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/cinema-4d/visual-feedback-of-animated-substances.html"
breadcrumb-title: ''
description: Ative a visualização animada no Cinema 4D para ver o feedback visual de materiais animados em Substance no visor.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Cinema 4D > Visual Feedback of Animated Substances
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Feedback visual de Substance animados
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 3%

---


# Feedback visual de Substance animados

Para ter feedback visual de um Substance animado no visor do Cinema 4D, a opção Visualização animada deve estar ativada para esses materiais.

Essa opção é encontrada no Editor de materiais no Editor (veja abaixo). Se um material foi criado usando o comando Criar material(is), essa opção será habilitada por padrão.

![](../../../assets/cinema-4d-13.png){width="500px"}


## Criando material(is)

Com o comando Criar materiais no Substance Asset Manager, você pode criar Cinema 4D de forma fácil e rápida usando um Substance.

Portanto, o seguinte mapeamento de canal será usado:

|  |  |
| --- | --- |
| **Canal de Saída do Substance** | **Canal de Material do Cinema 4D** |
| Difusão | Cor |
| Emissivo | Luminância |
| Reflexo | Reflexão |
| Ambiente | Ambiente |
| Relevo | Relevo |
| Opacidade | Alfa |
| Especular | Reflexão / Specular padrão |
| Altura | Deslocamento |
| Normal | Normal |

Essa relação só é usada para o comando Criar material(is) e o material que foi criado pode ser modificado subsequentemente. Convém usar esse comando para criar rapidamente uma material de base, que pode então ser ajustada ajustando apenas alguns canais.

Dentro do Substance Shader você não está limitado aos poucos canais de saída listados acima, mas na verdade você pode usar qualquer canal de saída que um Substance possa fornecer.

## Criando material(is) de Substance manualmente

Em vez de usar o comando Criar materiais, você também pode criar materiais manualmente usando o sombreador de Substance.

Basta selecionar o sombreador de Substance em um canal de material e arrastar o Substance que deseja usar. A próxima etapa é selecionar o canal de saída do Substance a ser usado neste sombreador e pronto.

Curtir:

![](../../../assets/cinema-4d-15.png){width="800px"}

Esse método oferece muita liberdade criativa e permite:

* Atribua canais de saída de Substance aos canais de Cinema 4D arbitrários. Não há necessidade de se restringir a usá-los apenas nos canais desejados.
* Atribua um único canal de saída de Substance a vários canais de Cinema 4D.
* Atribua canais de saída de vários Substance a um único Cinema 4D material.

## Limitações

* Os quadros-chave nos parâmetros de entrada de Substance são exibidos na linha do tempo, mas não no controle deslizante Powerslider do Cinema 4D (o controle deslizante Linha do tempo abaixo das viewports).
* Devido a uma limitação, nenhum perfil de cor personalizado deve ser usado em canais de saída de Substance.
* Em certas circunstâncias, as entradas de imagem de Substance serão interrompidas\
  O comando Mesclar... do Cinema 4D, que combina duas cenas em uma. Isso acontece se a cena a ser mesclada tiver Substance localizado em seu diretório de projeto com entradas de imagem referentes a imagens no diretório de projeto. Nesses casos, as entradas da imagem deverão ser revinculadas manualmente posteriormente.
* Se os Substance estiverem localizados na pasta do projeto (ou em outro local no caminho de pesquisa global), eles não funcionarão no Cineware. Nesse caso, elas são renderizadas em vermelho, como se o Substance estivesse ausente. Para contornar esse problema, os arquivos de Substance precisam ser armazenados fora do diretório do projeto, para que sejam referenciados por um caminho absoluto. Você pode usar o parâmetro Nome do arquivo para alterar o local do arquivo depois que os arquivos foram movidos para fora do caminho do projeto.
