---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/3d-applications/3ds-max/troubleshooting.html"
breadcrumb-title: ''
description: Diagnostique e resolva problemas com o plug-in Substance no 3ds Max usando o Ouvinte de scripts para mensagens de erro.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > Troubleshooting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Solução de problemas
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 1%

---


# Solução de problemas

O ouvinte de script pode ser usado para diagnosticar erros encontrados ao usar o plug-in. Para abrir o ouvinte de script, navegue até o Menu Script > Ouvinte de script. Quando ocorre um erro durante o uso do plug-in, uma mensagem de erro correspondente é impressa nesta janela do Ouvinte de script. Visite a [documentação oficial do Editor de Scripts](https://help.autodesk.com/view/3DSMAX/2023/ENU/?guid=GUID-C8019A8A-207F-48A0-985E-18D47FAD8F36) para obter mais informações.

Para relatar um erro, ingresse no canal #3dsmax-plugin no [servidor do Substance Discord](https://discord.com/invite/substance3d) ou visite as [comunidades de Adobe](https://community.adobe.com/t5/substance-3d-plugins/ct-p/ct-substance-3d-plugins?page=1&sort=latest_replies&lang=all&tabid=all&topics=label-autodesk3dsmax). Informações relevantes do registro do console e quaisquer etapas de reprodução para o problema podem ser incluídas nos relatórios.

## Problemas conhecidos

* *Substituir um .sbsar que usa uma saída difusa por um .sbsar que não usa um difuso leva à renderização em preto devido à desconexão do difuso ausente.*
  * Esse é o comportamento esperado para nós de várias saídas. Em vez de carregar esses .sbsars usando o mesmo nó, é recomendável usar nós de Substance diferentes para cada um.
