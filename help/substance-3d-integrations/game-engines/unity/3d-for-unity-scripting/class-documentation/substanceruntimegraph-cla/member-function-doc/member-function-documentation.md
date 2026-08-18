---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/game-engines/unity/substance-3d-for-unity-scripting/class-documentation/substanceruntimegraph-class/member-function-documentation.html"
breadcrumb-title: ''
description: Documentação detalhada de todas as funções membro da classe SubstanceRuntimeGraph no script Unity.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Substance 3D for Unity Scripting > Class Documentation > SubstanceRuntimeGraph Class > Member Function Documentation
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Documentação de Função do Membro
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 2%

---


# Documentação de Função do Membro

## AttachGraph()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.AttachGraph  

( SubstanceGraphSO graph ) [inline]
```


Anexa um novo objeto de gráfico a este manipulador de tempo de execução.

**Parâmetros**

|  |  |
| --- | --- |
| gráfico | Gráfico da substância de destino. |

### CreatePresetFromCurrentState()

```
string Adobe.Substance.Runtime.SubstanceRuntimeGraph.CreatePresetFromCurrentState ( ) [inline]
```


Salva o estado do gráfico atual em um XML predefinido.

**Retorna**

Predefinição criada usando o estado atual das entradas do gráfico.

### GetGeneratedTextures()

```
List< Texture2D > Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetGeneratedTextures ( ) [inline]
```


Retorna uma lista com todas as texturas de saída da instância do substance.

**Retorna**

Textura de saída.

### GetInputBool()

```
bool Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputBool ( string inputName ) [inline]
```


Obter Entrada Booleana Substance.

**Parâmetros**

|  |  |
| --- | --- |
| inputName | Nome da entrada no SBSAR. |


**Retorna**

Valor de entrada atual.

### GetInputColor()

```
Color Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputColor ( string inputName ) [inline]
```


Obter cor do Substance

**Parâmetros**

|  |  |
| --- | --- |
| inputName | Nome da entrada no SBSAR |


**Retorna**

Valor de entrada atual.

### GetInputDescription()

```
SubstanceInputDescription Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputDescription ( string inputName ) [inline]
```


Retorna a descrição de entrada completa do nome de entrada de destino.

**Parâmetros**

|  |  |
| --- | --- |
| inputName | Nome de entrada de destino. |


**Retorna**

Conclua a descrição de entrada da entrada de destino.

### GetInputFloat()

```
float Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputFloat ( string inputName ) [inline]
```


Obter entrada de flutuação de Substance

**Parâmetros**

|  |  |
| --- | --- |
| inputName | Nome da entrada no SBSAR |


**Retorna**

Valor de entrada atual.

### GetInputInt()

```
int Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputInt ( string inputName ) [inline]
```


Obter entrada Substance Int

**Parâmetros**

|  |  |
| --- | --- |
| inputName | Nome da entrada no SBSAR |


**Retorna**

Valor de entrada atual.

### GetInputString()

```
string Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputString ( string inputName ) [inline]
```


Obter entrada de cadeia de caracteres de Substance.

**Parâmetros**

|  |  |
| --- | --- |
| inputName | Nome da entrada no SBSAR |


**Retorna**

Inserir valor atual.

### GetInputVector2()

```
Vector2 Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector2 ( string inputName ) [inline]
```


Obter entrada Substance Vetor2

**Parâmetros**

|  |  |
| --- | --- |
| inputName | Nome da entrada no SBSAR |


**Retorna**

Valor de entrada atual.

### GetInputVector2Int()

```
Vector2Int Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector2Int ( string inputName ) [inline]
```


Obter matriz de 2 int.

**Parâmetros**

|  |  |
| --- | --- |
| inputName | Nome da entrada no SBSAR |


**Retorna**

Valor de entrada atual.

### GetInputVector3()

```
Vector3 Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector3 ( string inputName ) [inline]
```


Obter Entrada Vetor3 Substance.

**Parâmetros**

|  |  |
| --- | --- |
| inputName | Nome da entrada no SBSAR |


**Retorna**

Valor de entrada atual.

### GetInputVector3Int()

```
Vector3Int Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector3Int ( string inputName ) [inline]
```


Obter matriz de 3 int (valores x, y e z de Vetor3Int)

**Parâmetros**

|  |  |
| --- | --- |
| inputName | Nome da entrada no SBSAR |


**Retorna**

Valor de entrada atual.

### GetInputVector4()

```
Vector4 Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector4 ( string inputName ) [inline]
```


Obter entrada de vetor4 do Substance

**Parâmetros**

|  |  |
| --- | --- |
| inputName | Nome da entrada no SBSAR |


**Retorna**

Valor de entrada atual.

### GetInputVector4Int()

```
int[] Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetInputVector4Int ( string inputName ) [inline]
```


Obter matriz de 4 int (valores x, y, z &amp; w de Vetor4Int)

**Parâmetros**

|  |  |
| --- | --- |
| inputName | Nome da entrada no SBSAR |


**Retorna**

Valor de entrada atual.

### GetOutputTexture()

```
Texture2D Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetOutputTexture ( string outputName ) [inline]
```


Retorna a textura de saída de um determinado nome de saída.

**Parâmetros**

|  |  |
| --- | --- |
| outputName | Nome de saída. |


**Retorna**

Textura de saída.

### GetTexturesResolution()

```
Vector2Int Adobe.Substance.Runtime.SubstanceRuntimeGraph.GetTexturesResolution ( ) [inline]
```


Retorna a resolução de saída da textura da instância.

**Retorna**

Resolução de saída atual.

### HasInput()

```
bool Adobe.Substance.Runtime.SubstanceRuntimeGraph.HasInput ( string inputName ) [inline]
```


Retorna verdadeiro se esta instância do substance tiver uma entrada com um determinado nome.

**Parâmetros**

|  |  |
| --- | --- |
| inputName | Nome de entrada. |


**Retorna**

TRUE se a instância do substance tiver entrada com o nome fornecido.

### LoadPreset()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.LoadPreset ( string presetXML ) [inline]
```


Usa um XML predefinido para definir parâmetros de entrada de gráfico.

**Parâmetros**

|  |  |
| --- | --- |
| presetXML | Dados XML predefinidos. |

### RenderAsync()

```
Task Adobe.Substance.Runtime.SubstanceRuntimeGraph.RenderAsync ( ) [inline]
```


Renderiza a instância do substance de forma assíncrona.

**Retorna**

Tarefa que será concluída quando a renderização for concluída.

### SetInputBool()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputBool ( string inputName, 

bool value ) [inline]
```


Atualizar entrada de Substance booleano

**Parâmetros**

|  |  |
| --- | --- |
| inputName | Nome da entrada no SBSAR |
| valor | Valor usado para atualizar o parâmetro |

### SetInputColor()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputColor ( string inputName, 

Color value ) [inline]
```


Atualizar entrada de cor do Substance

**Parâmetros**

|  |  |
| --- | --- |
| inputName | Nome da entrada no SBSAR |
| valor | Valor usado para atualizar o parâmetro |

### SetInputFloat()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputFloat ( string inputName, 

float value ) [inline]
```


Atualizar entrada de flutuação de Substance

**Parâmetros**

|  |  |
| --- | --- |
| inputName | Nome da entrada no SBSAR |
| valor | Valor usado para atualizar o parâmetro |

### SetInputInt()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputInt ( string inputName, 

int value ) [inline]
```


Atualizar Entrada Substance Int

**Parâmetros**

|  |  |
| --- | --- |
| inputName | Nome da entrada no SBSAR |
| valor | Valor usado para atualizar o parâmetro |

### SetInputString()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputString ( string inputName, 

string value ) [inline]
```


Atualizar entrada da sequência de caracteres do Substance.

**Parâmetros**

|  |  |
| --- | --- |
| inputName | Nome da entrada no SBSAR |
| valor | Valor usado para atualizar o parâmetro |

### SetInputTexture()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputTexture (string inputName, 

Texture2D value ) [inline]
```


Atualizar Entrada Substance Texture2D.

**Parâmetros**

|  |  |
| --- | --- |
| inputName | Nome da entrada no SBSAR |
| valor | Valor usado para atualizar o parâmetro |

### SetInputVector2()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector2 ( string inputName, 

Vector2 value ) [inline]
```


Atualizar entrada Substance Vetor2

**Parâmetros**

|  |  |
| --- | --- |
| inputName | Nome da entrada no SBSAR |
| valor | Valor usado para atualizar o parâmetro |

### SetInputVector2Int()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector2Int ( string inputName, 

Vector2Int value ) [inline]
```


Atualize A Entrada Substance Vetor2Int.

**Parâmetros**

|  |  |
| --- | --- |
| inputName | Nome da entrada no SBSAR |
| valor | Valor usado para atualizar o parâmetro |

### SetInputVector3()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector3 ( string inputName, 

Vector3 value ) [inline]
```


Atualizar entrada de vetor3 do Substance

**Parâmetros**

|  |  |
| --- | --- |
| inputName | Nome da entrada no SBSAR |
| valor | Valor usado para atualizar o parâmetro |

### SetInputVector3Int()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector3Int ( string inputName, 

Vector3Int value ) [inline]
```


Atualize A Entrada Substance Vetor3Int.

**Parâmetros**

|  |  |
| --- | --- |
| inputName | Nome da entrada no SBSAR |
| valor | Valor usado para atualizar o parâmetro |

### SetInputVector4()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector4 ( string inputName, 

Vector4 value ) [inline]
```


Atualizar a entrada Substance Vetor4

**Parâmetros**

|  |  |
| --- | --- |
| inputName | Nome da entrada no SBSAR |
| valor | Valor usado para atualizar o parâmetro |

### SetInputVector4Int()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetInputVector4Int ( string inputName, 

int x, 

int y, 

int z, 

int w ) [inline]
```


Atualizar A Entrada Substance Vetor4Int

**Parâmetros**

|  |  |
| --- | --- |
| inputName | Nome da entrada no SBSAR |
| x | Valor usado para atualizar o parâmetro |
| y | Valor usado para atualizar o parâmetro |
| z | Valor usado para atualizar o parâmetro |
| w | Valor usado para atualizar o parâmetro |

### SetTexturesResolution()

```
void Adobe.Substance.Runtime.SubstanceRuntimeGraph.SetTexturesResolution ( Vector2Int size ) [inline]
```


Define a resolução de saída da textura da instância.

**Parâmetros**

|  |  |
| --- | --- |
| tamanho |  |
