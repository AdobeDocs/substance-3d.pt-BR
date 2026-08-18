---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/game-engines/unity/substance-3d-for-unity-scripting/class-documentation/substanceeditortools-256212996.html"
breadcrumb-title: ''
description: Documentação de referência para a classe SubstanceEditorTools usada para o gerenciamento de materiais de Substance no Unity.
helpx_creative_field: ""
helpx_description: Substance 3D Integrations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: SubstanceEditorFerramentas
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '104'
ht-degree: 0%

---


# SubstanceEditorFerramentas

## Referência da classe Adobe.SubstanceEditor.SubstanceEditorTools

Ferramentas e utilitários para usuários utilizarem em scripts do Editor.

Diagrama de herança de Adobe.SubstanceEditor.SubstanceEditorTools:

![](../../../../../assets/image2022-10-14-17-53-23.png)

### Funções Estáticas de Membro Público

```
• static void SetGraphFloatInput (SubstanceGraphSO graph, int inputId, float value)
```


Definir a entrada de flutuação do gráfico.

```
• static void SetGraphFloat2Input (SubstanceGraphSO graph, int inputId, Vector2 value)
```


Definir a entrada do gráfico float2.

```
• static void SetGraphFloat3Input (SubstanceGraphSO graph, int inputId, Vector3 value)
```


Definir a entrada do gráfico float3.

```
• static void SetGraphFloat4Input (SubstanceGraphSO graph, int inputId, Vector3 value)
```


Definir a entrada do gráfico float4.

```
• static void SetGraphIntInput (SubstanceGraphSO graph, int inputId, int value)
```


Definir entrada int do gráfico.

```
• static void SetGraphInt2Input (SubstanceGraphSO graph, int inputId, Vector2Int value)
```


Definir entrada int2 do gráfico.

```
• static void SetGraphInt3Input (SubstanceGraphSO graph, int inputId, Vector3Int value)
```


Definir entrada int3 do gráfico.

```
• static void SetGraphInt4Input (SubstanceGraphSO graph, int inputId, int value0, int value1, int value2, int value3)
```


Definir entrada int4 do gráfico.

```
• static void SetGraphInputString (SubstanceGraphSO graph, int inputId, string value)
```


Definir entrada de sequência de caracteres do gráfico.

```
• static void SetGraphInputTexture (SubstanceGraphSO graph, int inputId, Texture2D value)
```


Definir entrada de textura do gráfico.

```
• static void RenderGraph (SubstanceGraphSO graph)
```


Renderiza o gráfico de destino e atualiza seus ativos.

```
• static string CreatePresetFromCurrentState (SubstanceGraphSO graph)
```


Cria um XML predefinido a partir do estado atual do objeto de gráfico.

```
• static List< SubstanceGraphSO > GetGraphs (this SubstanceFileSO fileSO)
```


Retorna a lista de SubstanceGraphSOs associados a um SubstanceFileSO.
