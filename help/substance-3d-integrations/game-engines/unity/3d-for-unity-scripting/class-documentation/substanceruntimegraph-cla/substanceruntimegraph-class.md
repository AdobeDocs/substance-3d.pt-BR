---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/game-engines/unity/substance-3d-for-unity-scripting/class-documentation/substanceruntimegraph-class.html"
breadcrumb-title: ''
description: Documentação de referência para a classe SubstanceRuntimeGraph usada para operações de gráfico em tempo de execução no Unity.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Substance 3D for Unity Scripting > Class Documentation > SubstanceRuntimeGraph Class
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Classe SubstanceRuntimeGraph
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---


# Classe SubstanceRuntimeGraph

## Referência da classe Adobe.Substance.Runtime.SubstanceRuntimeGraph

Classe que fornece a funcionalidade de tempo de execução para modificar entradas em e renderizar gráficos de substância, permitindo que o Substance GrafoSO gere seus recursos em tempo de execução.

Diagrama de herança para Adobe.Substance.Runtime.SubstanceRuntimeGraph:

![](../../../../../assets/image2022-10-14-17-53-23-1.png)

### Funções de Membro Público

```
• void AttachGraph (SubstanceGraphSO graph)
```


Anexa um novo objeto de gráfico a este manipulador de tempo de execução.

```
• void SetInputFloat (string inputName, float value)
```


Atualizar entrada de flutuação de Substance

```
• float GetInputFloat (string inputName)
```


Obter entrada de flutuação de Substance

```
• void SetInputVector2 (string inputName, Vector2 value)
```


Atualizar entrada Substance Vetor2

```
• Vector2 GetInputVector2 (string inputName)
```


Obter entrada Substance Vetor2

```
• void SetInputVector3 (string inputName, Vector3 value)
```


Atualizar entrada de vetor3 do Substance

```
• Vector3 GetInputVector3 (string inputName)
```


Obter Entrada Vetor3 Substance.

```
• void SetInputVector4 (string inputName, Vector4 value)
```


Atualizar a entrada Substance Vetor4

```
• Vector4 GetInputVector4 (string inputName)
```


Obter entrada de vetor4 do Substance

```
• void SetInputColor (string inputName, Color value)
```


Atualizar entrada de cor do Substance

```
• Color GetInputColor (string inputName)
```


Obter cor do Substance

```
• void SetInputBool (string inputName, bool value)
```


Atualizar entrada de Substance booleano

```
• bool GetInputBool (string inputName)
```


Obter Entrada Booleana Substance.

```
• void SetInputInt (string inputName, int value)
```


Atualizar Entrada Substance Int

```
• int GetInputInt (string inputName)
```


Obter entrada Substance Int

```
• void SetInputVector2Int (string inputName, Vector2Int value)
```


Atualize A Entrada Substance Vetor2Int.

```
• Vector2Int GetInputVector2Int (string inputName)
```


Obter matriz de 2 int.

```
• void SetInputVector3Int (string inputName, Vector3Int value)
```


Atualize A Entrada Substance Vetor3Int.

```
• Vector3Int GetInputVector3Int (string inputName)
```


Obter matriz de 3 int (valores x, y e z de Vetor3Int)

```
• void SetInputVector4Int (string inputName, int x, int y, int z, int w)
```


Atualizar A Entrada Substance Vetor4Int

```
• int[ ] GetInputVector4Int (string inputName)
```


Obter matriz de 4 int (valores x, y, z &amp; w de Vetor4Int)

```
• void SetInputString (string inputName, string value)
```


Atualizar entrada da sequência de caracteres do Substance.

```
• string GetInputString (string inputName)
```


Obter entrada de cadeia de caracteres de Substance.

```
• SubstanceInputDescription GetInputDescription (string inputName)
```


Retorna a descrição de entrada completa do nome de entrada de destino.

```
• void SetInputTexture (string inputName, Texture2D value)
```


Atualizar Entrada Substance Texture2D.

```
• Vector2Int GetTexturesResolution ()
```


Retorna a resolução da saída da textura da instância.

```
• void SetTexturesResolution (Vector2Int size)
```


Define a resolução de saída da textura da instância.

```
• bool HasInput (string inputName)
```


Retorna verdadeiro se esta instância do substance tiver uma entrada com um determinado nome.

```
• List< Texture2D > GetGeneratedTextures ()
```


Retorna uma lista com todas as texturas de saída da instância do substance.

```
•  Texture2D GetOutputTexture (string outputName)
```


Retorna a textura de saída de um determinado nome de saída.

```
• void Render ()
```


Renderiza a instância do substance de forma síncrona.

```
• Task RenderAsync ()
```


Renderiza a instância do substance de forma assíncrona.

```
• void LoadPreset (string presetXML)
```


Usa um XML predefinido para definir parâmetros de entrada de gráfico.

```
• string CreatePresetFromCurrentState ()
```


Salva o estado do gráfico atual em um XML predefinido.

## Atributos públicos

```
• SubstanceGraphSO GraphSO
```


Instância da substância de destino.

## Funções de Membro Protegidas

```
• void Awake ()
```


Durante a ativação, o SubstanceRuntime será usado para criar uma instância para o SubstanceGraphSO anexado na substância

SDK.

```
• void Update ()
```


Verifique a renderização ConcurrentQueue para obter os resultados da renderização.

```
• void OnDestroy ()
```


Descarta o manipulador do SDK do substance.

## Propriedades

```
• Material DefaulMaterial [get]
```


Material principal gerado pela instância do substance.
