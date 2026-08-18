---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/substance-3d-for-unity-scripting.html"
breadcrumb-title: ''
description: Use a API do Substance 3D no Unity para gravar scripts que atualizam e alteram parâmetros de Substance no tempo de execução.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Substance 3D for Unity Scripting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance 3D para Script Unity
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---


# Substance 3D para Script Unity

Esta seção da documentação contém detalhes sobre a API do Substance 3D que fornecemos por meio do plug-in do Substance 3D para Unity. Usando as APIs de Substance, você pode gravar scripts para atualizar e alterar parâmetros de Substance no tempo de execução.

## Visão geral da API

O plug-in é dividido em 3 assemblies diferentes.

* Adobe.Substance
* Adobe.Substance.Editor
* Adobe.Substance.Runtime

### Adobe.Substance

Contém componentes compartilhados para interagir com o Substance SDK e gerar objetos Unity correspondentes. Ele também possui estruturas de dados de marshaling para comunicação entre C# e a API C++ do Substance SDK.

#### Adobe.Substance.Editor

Contém classes específicas do editor para manipular a exibição de informações sobre os objetos de Substance do Unity, bem como manipular o pipeline de importação para quando os arquivos sbsar são adicionados ao projeto. A classe SubstanceEditorEngine é um singleton que manipula o tempo de vida do mecanismo do substance e todas as suas instâncias gerenciadas.

#### Adobe.Substance.Runtime

Essa classe tem componentes que manipularão a criação e o gerenciamento de objetos de Substance durante a execução do tempo de execução. SubstanceRuntime é o equivalente da classe SubstanceEditorEngine para o tempo de execução. Ele manipulará a inicialização do mecanismo do substance, bem como a instanciação de qualquer instância do substance com a qual os scripts do usuário interagirão.

## Uso do tempo de execução

Para que as entradas da Instância de Substance sejam modificadas no tempo de execução, é necessário adicionar um SubstanceRuntime←- Material à sua cena (idealmente para o mesmo GameObject como material de substância). Essa classe atua como um auxiliar para configurar o material usando o singleton Adobe.Substance.Runtime.SubstanceRuntime que gerencia a instanciação de objetos do SDK de Substance no tempo de execução.

## Exemplos de código

O exemplo a seguir mostra como alterar parâmetros de entrada em tempo de execução usando SubstanceRuntimeGraph.

### Alterando Parâmetros

```
using System.Collections; 

using System.Collections.Generic; 

using UnityEngine; 

using Adobe.Substance.Runtime; 

public class scifiScript: MonoBehaviour { 

  public Adobe.Substance.Runtime.SubstanceRuntimeGraph mySubstance; 

  // Use this for initialization 

  void Start() { 

    UpdateSubstance(); 

  } 

  public void UpdateSubstance() { 

    // panel color 

    mySubstance.SetInputColor("paint_color", new Color(0.237 f, 0.834 f, 0.045 f, 1.0 f)); 

    // panel size 

    mySubstance.SetInputVector2("square_open", new Vector2(0.101 f, 0.209 f)); 

    // wear level 

    mySubstance.SetInputFloat("wear_level", 0.977 f); 

    // Submit async render. 

    mySubstance.RenderAsync(); 

  } 

}
```


Você também pode usar o SubstanceRuntimeGraph para ter acesso a informações de entrada e saída sobre o material do Substance.

#### Obter informações de entrada

```
using System.Collections; 

using System.Collections.Generic; 

using UnityEngine; 

using Adobe.Substance.Runtime; 

public class scifiScript: MonoBehaviour { 

  public Adobe.Substance.Runtime.SubstanceRuntimeGraph mySubstance; 

  // Use this for initialization 

  void Start() { 

    UpdateSubstance(); 

  } 

  public void UpdateSubstance() { 

    SubstanceInputDescription desc = mySubstance.GetInputDescription("paint_color"); 

    Debug.Log($ "Input: {desc.Identifier}"); 

    Debug.Log($ "Index: {desc.Index}"); 

    Debug.Log($ "Type: {desc.Type}"); 

    Debug.Log($ "Label: {desc.Label}"); 

  } 

}
```


O exemplo a seguir mostra como criar um menu de predefinição personalizado no editor com SubstanceEditorTools.

##### Criação de controles de predefinição.

```
using System.Collections; 

using System.Collections.Generic; 

using UnityEngine; 

using Adobe.Substance.Runtime; 

public class scifiScript: MonoBehaviour { 

  public Adobe.Substance.Runtime.SubstanceRuntimeGraph mySubstance; 

  // Use this for initialization 

  void Start() { 

    UpdateSubstance(); 

  } 

  public void UpdateSubstance() { 

    SubstanceInputDescription desc = mySubstance.GetInputDescription("paint_color"); 

    Debug.Log($ "Input: {desc.Identifier}"); 

    Debug.Log($ "Index: {desc.Index}"); 

    Debug.Log($ "Type: {desc.Type}"); 

    Debug.Log($ "Label: {desc.Label}"); 

  } 

}
```
