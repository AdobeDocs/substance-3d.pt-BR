---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/renderers/toolbag.html"
breadcrumb-title: ''
description: Use as saídas de Substance e metálicas no Toolbag 2 para visualização de material e renderização em tempo real.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Toolbag
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Toolbag
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 5%

---


# Toolbag

Esta página mostra como usar as saídas de aspereza/metálicas para o Toolbag 2.

A bolsa de ferramentas suporta os fluxos de trabalho specular/textura reluzente e metálico/aspereza.

O Substance 3D Painter usa o sombreador PBR metálico como padrão; no entanto, você também pode usá-lo com o sombreador de specular/brilho. Este fluxo de trabalho mostrará como usar as saídas metálicas do Toolbag 2. A bolsa de ferramentas é compatível com o fluxo de trabalho metálico.

[Baixar cena de exemplo](https://www.dropbox.com/s/qyed3un2zhtuibj/toolbag.zip?dl=0)

## Exportar do Painter

1. Ao usar o sombreador PBR metálico padrão, podemos exportar usando os canais de documento padrão + Normal + Predefinição de exportação para AO.  ***\*Os canais de documento exportam o Mapa normal com base na Configuração do Projeto. A bolsa de ferramentas requer o Mapa normal OGL. Você pode alternar o Formato Normal na Configuração do Projeto.***
1. Como alternativa, você pode criar uma configuração de exportação personalizada que use brilho

   ![](../../assets/settings-export.png){width="600px"}
1. É possível alterar o Formato normal para OpenGL antes de exportar.  **Editar>Configuração do Projeto**

   ![](../../assets/settings-normal-format.png)

## Configuração de material

1. Definir Refletividade como Metalidade
1. Definir Reflexo como GGX
1. Adicione as texturas aos canais apropriados, conforme mostrado no gráfico a seguir:

   | Substance 3D Painter Textura | Espaço de cores | Material da bolsa de ferramentas |
   | --- | --- | --- |
   | Cor de base | sRGB | Albedo |
   | Rugosidade | sRGB desativado | Microsuperfície - Brilho - Clique Inverter |
   | Metálico | sRGB desativado | Refletividade - Mapa do Metalness |
   | Normal | sRGB desativado | Normal |
   | Oclusão de ambiente | sRGB desativado | Oclusão |

![](../../assets/settings-toolbag.jpg){width="600px"}
