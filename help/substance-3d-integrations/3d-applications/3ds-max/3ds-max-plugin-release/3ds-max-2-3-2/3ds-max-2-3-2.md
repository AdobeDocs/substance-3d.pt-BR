---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-2-3-2.html"
breadcrumb-title: ''
description: Consulte as notas de versão do plug-in 3ds Max versão 2.3.2 para saber mais sobre novos recursos, melhorias e correções de erros.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds Max Plugin Release Notes > 3ds Max 2.3.2
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max 2.3.2
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---


# 3ds Max 2.3.2

Lançado em 8 de abril de 2020

Hoje nós lançamos a versão 2.3.2 do plugin, que é principalmente uma versão de correção de bug em cima de 2.3.1.

2.3.2 Versão:

* Atualizados os Substance Engine para 7.2.9
* Corrigido um problema com a renderização com falha do Redshift/VRay nos 3ds Max 2018, 2019 e 2020
* Os erros de declaração de depuração não serão mais exibidos
* O nó Substance2 agora tem corretamente as interfaces de script para iMultipleOutputChannelsWithValues
* A entrada de origem Substance no menu agora abrirá o Iniciador de Substance na guia Origem, se estiver instalado
* Os materiais Substance agora devem ser atualizados corretamente ao trabalhar com o renderizador Corona
* As saídas de Substance não são mais substituídas temporariamente por imagens quando usadas com VRay Próximo
* A caixa de diálogo de compatibilidade de renderização foi removida de aparecer automaticamente. Ela ainda estará disponível na caixa de diálogo de configurações, se necessário
* Corrigido um possível problema com a exportação de um fbx enquanto o material do substance era aplicado no 3ds Max 2021

Problemas conhecidos:

* No 3ds Max 2018, exportar um fbx com um material de Substance anexado ao objeto falhará no plug-in fbxmax.dlu. No momento, estamos conversando com a Autodesk para ver se há algo em nosso lado que possa ser feito ou se isso é uma limitação da versão mais antiga da integração do fbx. A solução alternativa anterior não era confiável e foi removida. Isso não ocorre no 3ds Max 2019 ou posterior.

Esta versão foi lançada para o 3ds Max 2018, 2019, 2020 e 2021.
