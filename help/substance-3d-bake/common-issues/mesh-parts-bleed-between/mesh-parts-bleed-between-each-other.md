---
helpx_url: "https://helpx.adobe.com/br/substance-3d-bake/common-issues/mesh-parts-bleed-between-each-other.html"
breadcrumb-title: ''
description: Evite que as partes da malha sangrem umas para as outras durante a cozedura usando a opção Corresponder por nome ou ajustando as distâncias.
helpx_creative_field: ""
helpx_description: bakers > Common Issues > Mesh parts bleed between each other
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: As partes da malha sangram entre si
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '131'
ht-degree: 0%

---


# As partes da malha sangram entre si

>[!WARNING]
>
> **Problema**
> 
> A geometria da malha sangra em outras partes e cria artefatos.
> 
> ![](../../assets/bleed-example.png)

>[!NOTE]
>
> **Explicação**
> 
> O processo de cozimento envia raios da superfície de malha de baixo-poli para atingir a malha de alto-poli para criar uma correspondência. Às vezes, os raios vão longe demais e atingem a geometria errada, criando o sangramento e os artefatos.

>[!NOTE]
>
> **Solução**
> 
> Algumas soluções estão disponíveis para evitar esse problema:
> 
> * Use o recurso [Correspondência por Nome](../../features/matching-by-name/matching-by-name.md) para isolar as malhas
> * Use uma [gaiola](https://helpx.adobe.com/br/substance-3d/unlisted/documentation/bake/cage-projection-172822982.html) para limitar a distância do raio.
> * Altere a distância padrão do raio nas configurações do padeiro comum para um valor mais baixo.
