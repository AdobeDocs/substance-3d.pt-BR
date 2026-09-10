---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/features/geometry-cache.html"
breadcrumb-title: ''
description: Use o cache de geometria para preservar os dados de malha pré-processados e acelerar significativamente as operações de cozimento subsequentes.
helpx_creative_field: ""
helpx_description: bakers > Features > Geometry Cache
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Cache de geometria
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 0%

---


# Cache de geometria

Na cozedura, as malhas são pré-processadas para serem limpas e convertidas em formato compatível com o processo de cozedura. O cache de geometria é uma maneira de preservar essa geometria pré-processada de uma forma que seja rápida de recarregar a fim de evitar refazer essa operação posteriormente (a menos que a malha de origem mude).

* Em **Substance Designer**, o cache de geometria é criado após a execução de um primeiro bake. O cache é então mantido na memória até que a janela do padeiro seja fechada.
* No **Substance Painter**, o cache de geometria é salvo como um arquivo com a extensão **assbin** ao lado do arquivo de origem após o primeiro cozimento.

Reutilizar o cache de geometria aumenta bastante o processo de cozimento, especialmente ao ajustar as configurações do padeiro para alcançar o resultado perfeito.
