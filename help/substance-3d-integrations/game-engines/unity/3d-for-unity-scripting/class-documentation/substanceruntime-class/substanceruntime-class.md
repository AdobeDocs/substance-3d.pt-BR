---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/game-engines/unity/substance-3d-for-unity-scripting/class-documentation/substanceruntime-class.html"
breadcrumb-title: ''
description: Documentação de referência para a classe SubstanceRuntime usada para operações de material de Substance em tempo de execução no Unity.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Substance 3D for Unity Scripting > Class Documentation > SubstanceRuntime Class
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Classe SubstanceRuntime
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '134'
ht-degree: 1%

---


# Classe SubstanceRuntime

## Referência de classe Adobe.Substance.Runtime.SubstanceRuntime

Classe singleton que manipula a inicialização do mecanismo Substance e é usada para obter manipuladores nativos para instâncias do substance.\
Diagrama de herança para Adobe.Substance.Runtime.SubstanceRuntime:

![](../../../../../assets/image2022-6-22-14-35-28.png)

### Funções de Membro Público

```
• SubstanceNativeGraph InitializeInstance (SubstanceGraphSO substanceInstance)
```


Cria um identificador do SDK do Substance para um determinado SubstanceGraphSO.

### Propriedades

```
• static SubstanceRuntime Instance [get]
```


Instância de singleton.

### Descrição detalhada

Classe singleton que manipula a inicialização do mecanismo Substance e é usada para obter manipuladores nativos para instâncias do substance.

### Documentação de Função do Membro

#### InitializeInstance()

```
SubstanceNativeGraph Adobe.Substance.Runtime.SubstanceRuntime.InitializeInstance  

( SubstanceGraphSO substanceInstance ) [inline]
```


Cria um identificador do SDK do Substance para um determinado SubstanceGraphSO.

**Parâmetros**

|  |  |
| --- | --- |
| substanceInstance | SubstanceGraphSO de destino |


**Retorna**

Identificador que se comunica com o Substance SDK

### Documentação de propriedade

#### Instância

```
SubstanceRuntime Adobe.Substance.Runtime.SubstanceRuntime.Instance [static], [get]
```


Instância de singleton.

Instância singleton global.

>[!NOTE]
>
> O NativeGraph.InRenderWork destina-se apenas a uso interno para comunicação com o Substance Engine e não deve ser usado para workflows personalizados.
