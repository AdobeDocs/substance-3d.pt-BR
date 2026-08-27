---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/transferred-texture-from-mesh.html"
breadcrumb-title: ''
description: Transfira texturas entre malhas com base em seus UVs, incluindo suporte para conversões de mapa normais.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Transferred Texture from Mesh
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Textura transferida da malha
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 3%

---


# Textura transferida da malha

A textura transferida do mesh baker permite converter uma textura de uma malha para outra com base em seus respectivos UVs. Este padeiro também suporta a transferência ou mapas normais (que requerem conversões especiais). Para funcionar, ambas as malhas precisam de definições UV.

**Disponível em:**

* Substance Designer
* Substance Automation Toolkit

## Parâmetros

| *Parâmetro* | *Descrição* |
| --- | --- |
| **Arquivo de textura** | Caminho para o arquivo de textura de entrada que será transferido. |
| **Conjunto UV** | UVs de malha para usar na malha de alto polígono para ler a textura e projetá-la na malha de baixo polígono. |
| **Modo de Filtragem** | Define como a interpolação de pixels da textura deve ser feita.Valores possíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Mais próximo</strong>: nenhuma interpolação, use o pixel mais próximo encontrado para uma determinada posição. Precisa, mas pode criar suavização.</li><li data-preserve-html="true"><strong>Bilinear</strong> (padrão): use os quatro pixels mais próximos para uma determinada posição. Sem aliases, mas pode ficar desfocado.</li></ul> |
| **Mapa Normal** | Se ativada, indica ao padeiro que a textura de entrada a ser transferida é um mapa normal. Isso indica que o padeiro deve aplicar conversões especiais à textura para torná-la compatível com a malha de destino. |
| **Tipo de Mapa** | Define que tipo de mapa normal é a textura de entrada.Valores possíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Espaço Mundial</strong></li><li data-preserve-html="true"><strong>Espaço Tangente</strong> (padrão)</li></ul> |
| **Orientação Normal** | Define o formato normal da textura de entrada se **Tipo de Mapa** estiver definido como **Espaço Tangente**.Valores possíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>OpenGL</strong></li><li data-preserve-html="true"><strong>DirectX</strong> (padrão)</li></ul> |
