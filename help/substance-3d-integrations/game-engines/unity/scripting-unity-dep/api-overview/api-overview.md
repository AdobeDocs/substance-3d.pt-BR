---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/scripting-in-unity-deprecated/api-overview.html"
breadcrumb-title: ''
description: Visão geral de referência da API do Substance Unity obsoleta para projetos herdados e necessidades de script.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Scripting in Unity (Deprecated) > API Overview
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Visão geral da API
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 0%

---


# Visão geral da API

## Substance.Jogo

```
Using Substance.Game
```


Substance.Game é o assembly que contém as classes usadas para scripts. Estas classes são as seguintes:

**Substance.Game.**&#x200B;**Substance**: Referencia o sbsar

**Substance.Game.SubstanceGraph**: gráfico individual no sbsar.*(usado para ser ProceduralMaterial no Unity 2017)*

## Processo de script

1. Criar uma instância do SubstanceGraph
1. Defina parâmetros na instância do gráfico.
1. Enfileirar o Substance para renderização: QueueForRender() adicionará o gráfico do substance a uma fila. Essa lista será processada na próxima chamada para RenderAsync ou RenderSync.

### Parâmetros de instância de gráfico

```
// panel color 

mySubstance.SetInputColor("paint_color", color); 

 

// panel size 

mySubstance.SetInputVector2("square_open", panelSize); 

 

// wear level 

mySubstance.SetInputFloat("wear_level", wearLevel);
```


O valor entre aspas é o Identificador de parâmetro definido em Substance Designer.

No Inspetor de unidade, você pode passar o mouse sobre um parâmetro para revelar uma dica de ferramenta que mostra o nome do Identificador definido em Substance Designer.

![](../../../../assets/tooltip-6.png)

### Enfileirar a substância para renderização

```
// queue the substance to render 

mySubstance.QueueForRender(); 

 

//render all substances async 

Substance.Game.Substance.RenderAsync();
```


![](../../../../assets/unityscript.gif)

>[!NOTE]
>
> Atualmente, só oferecemos suporte à arquitetura x86\_64. Você precisa definir x86\_64 nas Configurações de compilação

![](../../../../assets/arch.png)
