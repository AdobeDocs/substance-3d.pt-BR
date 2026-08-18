---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/3d-applications/maya/substance-output-node.html"
breadcrumb-title: ''
description: Entenda como os nós de saída de Substance funcionam no Maya para conectar texturas computadas a redes sombreadoras.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Substance Output Node
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Nó de saída do Substance
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '137'
ht-degree: 0%

---


# Nó de saída do Substance

O nó de saída do Substance é uma referência à textura computada do Substance Engine. Ele está conectado ao nó Substance. Quando uma saída é criada no nó Substance, o mecanismo Substance computa a textura e esses dados são mantidos como RAM. Se estiver usando o mecanismo da GPU, os dados serão calculados na GPU e enviados de volta à memória usando o mecanismo de mesclagem da GPU de Substance. As saídas no nó do Substance que não estão ativadas não são computadas.

![](../../../assets/outputnode.png)

Neste nó, você pode ver as informações de Saída, como Identificador, Rótulo e Uso definidos na saída em Substance Designer. Este nó também permite preparar a textura para o disco na seção Cache de saída.
