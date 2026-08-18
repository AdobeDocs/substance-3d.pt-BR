---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/renderers/keyshot.html"
breadcrumb-title: ''
description: Use materiais de Substance no renderizador de captura de tela para visualização do produto com mapas de textura exportados.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Renderers > Keyshot
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Keyshot
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 8%

---


# Keyshot

*Keyshot 6.1.72*[ Baixar Cena De Exemplo](https://www.dropbox.com/s/rvjsbbcx7c74aah/keyshot.zip?dl=0)

## Exportar Substance Painter

1. Para o Keyshot, você precisará configurar uma predefinição de exportação usando Difusa, Reflexão, Metálica, Aspereza e Normal (X direto).

   ![](https://helpx-prod.scene7.com/is/image/HelpxProd/key-01?$png$&jpegSize=300&wid=1794)

## Configuração Avançada de Material

Você usará 2 materiais avançados. Uma será para metais e a outra para dielétricos.

1. Defina o material como Avançado e crie um gráfico do material.

   **Metálico:**\
   a) Defina o índice de refração como 10\
   b) Defina os mapas conforme indicado na tabela abaixo

   | textura do Substance Painter | Canal de material avançado |
   | --- | --- |
   | Difusão | Difusão |
   | Metálico | Opacidade |
   | Normal | Bump \*Normal Ativado |
   | Rugosidade | Rugosidade |
   | Reflexo | Especular |

1. Criar um novo material avançado

   **Dielétrico:**\
   a) Defina o índice de refração como 1,5\
   b) Defina os mapas conforme indicado na tabela abaixo

   | textura do Substance Painter | Canal de material avançado |
   | --- | --- |
   | Difusão | Difusão |
   | Normal | Bump \*Normal Ativado |
   | Rugosidade | Rugosidade |
   | Reflexo | Especular |

1. Obtenha a saída do Material avançado metálico e adicione-a ao + do Material avançado dielétrico. Isso criará um campo Rótulo no material.

   ![](../../assets/key-02.png)
