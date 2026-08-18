---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/common-questions/texture-baked-outside-of-substance-software-looks-incorrect.html"
breadcrumb-title: ''
description: Solucione problemas de porque as texturas assadas fora do software de Substance parecem incorretas e saiba como corrigir problemas de espaço de cores.
helpx_creative_field: ""
helpx_description: bakers > Common Questions > Texture baked outside of Substance software looks incorrect
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: A textura cozida fora do software do Substance parece incorreta
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 0%

---


# A textura cozida fora do software do Substance parece incorreta

>[!WARNING]
>
> **Pergunta**
> 
> Por que a textura que cozinhei com um aplicativo externo e não os Substance Bakers parecem incorretos no Substance Painter?

>[!NOTE]
>
> **Solução**
> 
> Não há solução imediata para esse problema, pois muitos fatores podem contribuir para o problema:
> 
> * Verifique se o formato normal entre o software do Substance e o aplicativo externo é o mesmo. O OpenGL é [X+, Y+, Z+] e o DirectX é [X+, Y-, Z+]
>   * No Substance Painter, o formato normal pode ser alterado na [configuração de projeto](https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/interface/project-configuration).
>   * No Substance Designer, o formato normal pode ser alterado nas [preferências de projeto](https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/workspace/preferences/project-settings).
> * Verifique se a malha foi triangulada antes de assar e importe-a no software Substance. Consulte [esta página](../../guides/triangulating-before-bak/triangulating-before-baking.md) para obter mais informações.
