---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/3d-applications/modo/working-with-normals.html"
breadcrumb-title: ''
description: Defina as configurações normais de orientação do mapa no MODO para garantir a renderização correta do mapa normal com materiais Substance.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Working with Normals
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Trabalhando com normais
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '151'
ht-degree: 0%

---


# Trabalhando com normais

Trabalhar com dados normais - Definir a orientação correta

Os Substance do Stock são criados para usar a orientação normal DX. No entanto, o MODO usa OGL. Você pode inverter o normal definindo o parâmetro Formato normal como 1.0. O plug-in Substance interpretará apenas os parâmetros definidos no Substance. Você pode encontrar um Substance que não tem o parâmetro “normal\_format”, pois cabe ao autor do Substance adicionar esse controle a Substance personalizados. Se você encontrar um Substance que não tem esse parâmetro, pode virar o canal verde na camada de textura do mapa normal para corrigir a orientação.

>[!NOTE]
>
> Virar o canal de verde é apenas se o Substance tiver a orientação normal errada e o autor não tiver criado um controle para inverter o normal nos parâmetros de Substance

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![](../../../assets/normal-1.png)

</td>
<td style="border: 0;" valign="top">

![](../../../assets/invert-2.png)

</td>
</tr>
</table>
