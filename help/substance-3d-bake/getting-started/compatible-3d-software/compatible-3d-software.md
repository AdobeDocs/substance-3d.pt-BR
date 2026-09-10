---
helpx_url: "https://helpx.adobe.com/br/substance-3d-bake/getting-started/compatible-3d-software.html"
breadcrumb-title: ''
description: Descubra qual software 3D é compatível com o Substance Bakers e aprenda a preparar malhas para obter os melhores resultados de fça bake.
helpx_creative_field: ""
helpx_description: bakers > Getting Started > Compatible 3D software
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Software 3D compatível
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 2%

---


# Software 3D compatível

A maioria dos softwares 3D é compatível com os Substance Bakers, desde que eles exportem geometria de malha como polígonos em formatos de arquivo compatíveis com os aplicativos.

No entanto, nem todos os softwares estão no mesmo nível em termos de recursos e qualidade ao exportar essas malhas. É por isso que é importante limpar uma malha corretamente e certificando-se de que será compatível com os padeiros. Para obter mais informações sobre como preparar uma malha, consulte os vários [Guias](../../guides/performances-and-opt/performances-and-optimizations.md).

## Compatibilidade de software

Veja abaixo uma lista dos softwares 3D mais conhecidos e suas compatibilidades com os baker:

| *Nome* | *Status* |
| --- | --- |
| **Mesclador** | Compatível: requer nivelar modificadores antes da exportação. |
| **Maya** | Compatível: requer um transformo de congelamento e exclui o histórico antes da exportação. |
| **3DS Máx** | Compatível: requer uma redefinição do xForm antes da exportação. |
| **MODO** | Compatível: é recomendado usar o exportador da aba Jogo definido como “Malha estática irreal”. |
| **Cinema 4D** | Compatível: requer nivelar modificadores antes da exportação. |
| **zBrush** | Não compatível: malhas de baixo polígono precisam ser processadas e limpas em outro aplicativo 3D primeiro. Compatível: malhas de alto-poli para fazer bake. |

## Formato de arquivo

Ao assar a geometria, é importante levar em conta o formato de arquivo usado também. O formato de arquivo definirá a quantidade de informações que será salva na malha.

Ter muita informação às vezes pode ser prejudicial e levar a erros. Geralmente, recomendamos experimentar formatos de arquivo diferentes quando ocorrem erros, pois isso pode ser uma maneira fácil de solucionar problemas e determinar se o culpado está no próprio baker ou se vem do software 3D.

Confira abaixo uma visão geral rápida dos dois formatos de arquivo mais comuns compatíveis com os baker:

| Formato de arquivo | Informações |
| --- | --- |
| **FBX** | Autodesk FBX (Filmbox) é o principal formato de arquivo usado pela Autodesk Software, que pode ser escrito como texto ou binário.  Ele suporta :<ul data-preserve-html="true"><li data-preserve-html="true">UVs (conjuntos múltiplos)</li><li data-preserve-html="true">Vértice, Tangente e Binormais</li><li data-preserve-html="true">Cores do vértice</li><li data-preserve-html="true">Face triangular, face quádrupla e face N-Gon</li><li data-preserve-html="true">Câmeras</li><li data-preserve-html="true">Luzes</li><li data-preserve-html="true">Subdivisões da malha</li><li data-preserve-html="true">Suavização de grupos</li><li data-preserve-html="true">Informações sobre materiais (como cores)</li><li data-preserve-html="true">Bitmap</li></ul> |
| **OBJ** | Wavefront OBJ é um formato de arquivo com base em texto muito simples que oferece suporte para :<ul data-preserve-html="true"><li data-preserve-html="true">UVs (apenas um conjunto)</li><li data-preserve-html="true">Normais de vértice</li><li data-preserve-html="true">Cores de vértice (somente se exportadas do Pixologic zBrush)</li><li data-preserve-html="true">Face triangular, face quádrupla e face N-Gon</li><li data-preserve-html="true">Cor do material (se o arquivo <strong>mtl</strong> estiver presente)</li></ul> |
