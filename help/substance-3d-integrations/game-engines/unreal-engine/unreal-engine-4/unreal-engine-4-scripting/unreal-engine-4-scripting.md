---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/unreal-engine-4-scripting.html"
breadcrumb-title: ''
description: Use a API de script do Substance Unreal Engine 4 para gerenciar materiais de Substance de forma programática em seus projetos.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Unreal Engine 4 Scripting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Script do Unreal Engine 4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 0%

---


# Script do Unreal Engine 4

O Substance no plug-in Unreal Engine pode ser programado para script. Os métodos são listados e anotados no arquivo SubstanceGraphInstance.h do plug-in, que normalmente é encontrado no seguinte diretório ao instalar o plug-in no marketplace:

* **Instalação do mecanismo**: [UE\_4.X.X local]\Engine\Plugins\Marketplace\Substance\Source\SubstanceCore\Classes\SubstanceGraphInstance.h
* **Instalação do projeto**: [local da pasta do projeto]\Plugins\Runtime\Substance\Source\SubstanceCore\Classes\SubstanceGraphInstance.h

  ![](../../../../assets/substancegraphinstance.png)

`BlueprintCallable` indica que o método também é utilizável no Editor de Blueprint.

## Scripts no Editor de Python do Unreal Engine

Ao usar os métodos listados no arquivo SubstanceGraphInstance.h no editor Python do Unreal Engine, eles devem ser convertidos de Pascal Case para Snake Case (com letras minúsculas e sublinhado entre cada palavra). Por exemplo, `SetInputColor` torna-se `set_input_color`.

O Editor Python no Unreal Engine pode ser acessado em Janela > Ferramentas do desenvolvedor > Log de saída e definindo o menu suspenso inferior esquerdo como Python.

## Exemplos de scripts

Abaixo está um conjunto de scripts de exemplo que podem ser usados no Editor de Python.

## Criar um material de Substance

```
## Python example on creating a Substance material.

 

import unreal 

 

## Create factory

sf = unreal.SubstanceFactory() 

factory = sf.import_archive("/Game", "C:/4d/unreal/stylized_lava_cracked.sbsar") 

graph_descs = factory.get_graph_descs() 

mats = unreal.SubstanceUtility.get_substance_included_materials() 

 

## Create graph instance

for graph_desc in graph_descs: 

    print(graph_desc) 

## You could name based on label or on index or another way

    graph_name = "/Game/FirstInstance_" + graph_desc.label 

    material_name = "/Game/FirstMaterial_" + graph_desc.label 

## graph_name = f"/Game/FirstInstance_{graph_desc.index}"

## material_name = f"/Game/FirstMaterial_{graph_desc.index}"

    graph = factory.create_graph_instance(graph_desc, graph_name) 

    graph.create_outputs() 

    graph.create_material(material_name, mats[0]) 

    graph.set_input_color("obsidian_color", unreal.LinearColor(0, 0, 1)) 

    graph.set_input_color("lava_color", unreal.LinearColor(0, 1, 0)) 

    graph.prepare_outputs_for_save() 

    graph.render_sync() 

    graph.save_all_outputs(True)
```


## Criar um único gráfico de um material de Substance

```
## Python example on creating a Substance material.

 

import unreal 

 

## Create factory

sf = unreal.SubstanceFactory() 

factory = sf.import_archive("/Game", "C:/4d/unreal/stylized_lava_cracked.sbsar") 

graph_descs = factory.get_graph_descs() 

mats = unreal.SubstanceUtility.get_substance_included_materials() 

 

## Create only 1 graph instance

graph_desc = graph_descs[0] 

print(graph_desc) 

graph_name = "/Game/MyGraphInstance" 

material_name = "/Game/MyMaterial" 

graph = factory.create_graph_instance(graph_desc, graph_name) 

graph.create_outputs() 

graph.create_material(material_name, mats[0]) 

graph.set_input_color("obsidian_color", unreal.LinearColor(0, 1, 1)) 

graph.set_input_color("lava_color", unreal.LinearColor(1, 0, 0)) 

graph.prepare_outputs_for_save() 

graph.render_sync() 

graph.save_all_outputs(True)
```


## Crie várias instâncias de um material de Substance com diferentes parâmetros.

```
## Python example on creating mulitple Substance materials.

 

import unreal 

 

## Create factory. Should only need 1 factory, even if multiple instances are created

sf = unreal.SubstanceFactory() 

factory = sf.import_archive("/Game", "C:/4d/unreal/stylized_lava_cracked.sbsar") 

graph_descs = factory.get_graph_descs() 

mats = unreal.SubstanceUtility.get_substance_included_materials() 

 

## Create first graph instance

for graph_desc in graph_descs: 

    graph_name = "/Game/FirstInstance_" + graph_desc.label 

    material_name = "/Game/FirstMaterial_" + graph_desc.label 

    graph = factory.create_graph_instance(graph_desc, graph_name) 

    graph.create_outputs() 

    graph.create_material(material_name, mats[0]) 

    graph.set_input_color("obsidian_color", unreal.LinearColor(0, 0, 1)) 

    graph.set_input_color("lava_color", unreal.LinearColor(0, 1, 0)) 

    graph.prepare_outputs_for_save() 

    graph.render_sync() 

    graph.save_all_outputs(True) 

 

## Create second graph instance

for graph_desc in graph_descs: 

    graph_name = "/Game/SecondInstance_" + graph_desc.label 

    material_name = "/Game/SecondMaterial_" + graph_desc.label 

    graph = factory.create_graph_instance(graph_desc, graph_name) 

    graph.create_outputs() 

    graph.create_material(material_name, mats[0]) 

    graph.set_input_color("obsidian_color", unreal.LinearColor(1, 0, 1)) 

    graph.set_input_color("lava_color", unreal.LinearColor(1, 1, 0)) 

    graph.prepare_outputs_for_save() 

    graph.render_sync() 

    graph.save_all_outputs(True)
```


## Duplicar um Gráfico do Substance

```
## Python example on duplicating a Subtance material.

 

import unreal 

 

## Create factory

sf = unreal.SubstanceFactory() 

factory = sf.import_archive("/Game", "C:/4d/unreal/stylized_lava_cracked.sbsar") 

graph_descs = factory.get_graph_descs() 

mats = unreal.SubstanceUtility.get_substance_included_materials() 

 

## Create first graph

for graph_desc in graph_descs: 

    print(graph_desc) 

    graph_name = "/Game/FirstGraph_" + graph_desc.label 

    material_name = "/Game/FirstMaterial_" + graph_desc.label 

    graph = factory.create_graph_instance(graph_desc, graph_name) 

    graph.create_outputs() 

    graph.create_material(material_name, mats[0]) 

    graph.set_input_color("obsidian_color", unreal.LinearColor(0, 0, 1)) 

    graph.set_input_color("lava_color", unreal.LinearColor(0, 1, 0)) 

    graph.prepare_outputs_for_save() 

    graph.render_sync() 

 

## Duplicate graph

new_material_name = "/Game/SecondMaterial" 

new_graph = graph.duplicate() 

new_graph.create_outputs() 

new_graph.create_material(new_material_name, mats[0]) 

new_graph.prepare_outputs_for_save() 

new_graph.render_sync()
```
