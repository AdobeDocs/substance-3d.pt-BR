---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/maya/maya-scripting.html"
breadcrumb-title: ''
description: Use a API do Substance Maya para criar e gerenciar materiais de Substance em seus fluxos de trabalho do Maya.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Maya Scripting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Maya Scripting
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 0%

---


# Maya Scripting

O plug-in Substance no Maya pode ser criado com script. Uma API exposta permite que comandos Substance sejam usados em scripts para criar e gerenciar materiais de Substance. Você pode acessar os comandos disponíveis indo até as informações do plug-in.

***Windows>Gerenciador de Configurações/Preferências/Plug-in e procure o arquivo substancemaya.mll.***

Clique no botão “i” para ver os comandos disponíveis

![](../../../assets/script-7.png)

## Exemplo de script:

Esse script carregará um arquivo sbsar e aplicará o fluxo de trabalho de renderização Arnold à malha selecionada. Para usar o script, siga o exemplo listado aqui.

1. copie e cole o código em uma aba Python do editor de script.
1. Selecionar e aplicar malha no visor
1. Selecione o texto na aba Python e pressione “ctrl + enter”
1. Na janela, procure um arquivo sbsar.

```
import maya.cmds as cmds 

 

def _connect_place2d(substance_node): 

    """ Connects the place2d texture node to the Substance node """ 

    place_node = cmds.shadingNode('place2dTexture', asUtility=True) 

 

    connect_attrs = [('outUV', 'uvCoord'), ('outUvFilterSize', 'uvFilterSize')] 

 

    for out_attr, in_attr in connect_attrs: 

        cmds.connectAttr('{}.{}'.format(place_node, out_attr), 

                         '{}.{}'.format(substance_node, in_attr)) 

 

def _find_shading_group(node): 

    """ Walks the shader graph to find the shading group """ 

    result = None 

 

    connections = cmds.listConnections(node, source=False) 

 

    if connections: 

        for connection in connections: 

            if cmds.nodeType(connection) == 'shadingEngine': 

                result = connection 

            else: 

                result = _find_shading_group(connection) 

                if result is not None: 

                    break 

 

    return result 

 

def _apply_substance_workflow_to_selected(substance_file, workflow): 

    """ Imports a mesh into Maya and applies the shader from a 

        Substance workflow to it """ 

    geometry = cmds.ls(geometry=True) 

 

## Create the substance node and connect the place2d texture node

    substance_node = cmds.shadingNode('substanceNode', asTexture=True) 

    _connect_place2d(substance_node) 

 

## Load the Substance file

    cmds.substanceNodeLoadSubstance(substance_node, substance_file) 

 

## Apply the workflow

    cmds.substanceNodeApplyWorkflow(substance_node, workflow=workflow) 

 

## Acquire the shading group and apply it to the mesh

    shading_group = _find_shading_group(substance_node) 

 

    cmds.select(geometry) 

    cmds.hyperShade(assign=shading_group) 

 

def demo_load_sbsar_workflow(): 

    """ Acquires an sbsar from a file dialog, loading and applying it to 

        any selected mesh """ 

    file_filter = 'Substance (*.sbsar);;' 

 

    files = cmds.fileDialog2(cap='Select a Substance file', fm=1, dialogStyle=2, 

                             okc='Open', fileFilter=file_filter) 

 

    if files: 

        substance_file = files[0] 

        _apply_substance_workflow_to_selected(substance_file, 

                                              cmds.substanceGetWorkflow()) 

 

if __name__ == '__main__': 

    demo_load_sbsar_workflow()
```


Uma API exposta permite que comandos Substance sejam usados em scripts
