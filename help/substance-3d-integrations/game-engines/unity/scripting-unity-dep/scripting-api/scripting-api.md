---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/scripting-in-unity-deprecated/scripting-api.html"
breadcrumb-title: ''
description: Documentação de referência para a API de script de unidade de Substance obsoleta para suporte a projeto herdado.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Scripting in Unity (Deprecated) > Scripting API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: API de script
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '1074'
ht-degree: 1%

---


# API de script

## Substance na API do Unity - 2.2.0

## parâmetros de material de Substance

| Método público | Descrição | Parâmetro |
| --- | --- | --- |
| **float** público *GetInputFloat*(**cadeia** inputName) | Obter Entrada De Substance **Precisão decimal** | **Cadeia** *inputName* Nome da entrada no SBSAR |
| público **int** *SetInputFloat*(**cadeia** inputName, valor **float**) | Atualizar entrada de Substance **Precisão decimal** | **Cadeia de caracteres** i *nputName* Nome da entrada na **Precisão decimal** *valor* SBSAR usada para atualizar o parâmetro |
| public **void** *SetInputVector2*(**cadeia** inputName, valor **Vetor2**) | Atualizar Entrada de Substance **Vetor2** | **Cadeia de caracteres** *inputName* Nome da entrada nos valores SBSAR **Vetor2** *entrada* usados para atualizar o parâmetro |
| público **vetor2** *GetInputVector2*(**cadeia** inputName) | Obter Entrada de Substance **Vetor2** | **Cadeia de caracteres** “inputName” Nome da entrada no SBSAR |
| public **void** *SetInputVector3*(**cadeia** inputName, valor **Vetor3**) | Atualizar Entrada do Substance **Vetor3** | **Cadeia de caracteres** *inputName* Nome da entrada nos valores SBSAR **Vetor3** *valor* usados para atualizar o parâmetro |
| **vetor3** público *GetInputVector3*(**cadeia** inputName) público | Obter Entrada de Substance **Vetor3** | **Cadeia** *inputName* Nome da entrada no SBSAR |
| public **void** *SetInputVector4*(**cadeia** inputName, valor **Vetor4**) | Atualizar Entrada de Substance **Vetor4** | **Cadeia de caracteres** *inputName* Nome da entrada nos valores **Vetor4** *value* SBSAR usados para atualizar o parâmetro |
| público **vetor4** *GetInputVector4*(**cadeia** inputName) | Obter Entrada De Substance **Vetor4** | **Cadeia** inputName Nome da entrada no SBSAR |
| public **void** *SetInputColor*(**cadeia** inputName, valor **Cor**) | Atualizar Entrada De Substance **Cores** | **Cadeia** inputName Nome da entrada no Valor **Cor** SBSAR usado para atualizar o parâmetro |
| **color** *GetInputColor*(**string** inputName, **int** dataType) público | Obter Substance **Cor** | **String** *inputName* Nome da entrada no SBSAR **Int** *dataType* |
| public **void** *SetInputBool*(**cadeia** inputName, valor **bool**) | Atualizar entrada do Substance **booleano** | **Cadeia de caracteres** *inputName* Nome da entrada no valor **Bool** *value* de SBSAR usado para atualizar o parâmetro |
| público **bool** *GetInputBool*(**cadeia** inputName) | Obter Entrada Substance **Booleana** | **Cadeia** *inputName* Nome da entrada no SBSAR |
| public **void** *SetInputInt*(**cadeia** inputName, valor **int**) | Atualizar Entrada Do Substance **Int** | **Cadeia de caracteres** *inputName* Nome da entrada no valor **Int** *SBSAR* usado para atualizar o parâmetro |
| público **int** *GetInputInt*(**cadeia** inputName) | Obter Entrada De Substance **Int** | **Cadeia** *inputName* Nome da entrada no SBSAR |
| public **void** *SetInputVector2Int*(**string** inputName, **int** x, **int** y) | Atualizar A Entrada Do Substance **Vetor2Int** | **Cadeia de caracteres** *inputName* Nome da entrada no Valor **Int** *x* SBSAR usado para atualizar o parâmetro **Int** y Valor usado para atualizar o parâmetro |
| **int[] Substance.Game.SubstanceGraph**.*GetInputVector2Int*( string inputName) | Obter matriz de 2 int (valores x &amp; y de Vetor2Int) | **Cadeia de caracteres** *inputName* Nome da entrada no Valor **Int** *x* SBSAR usado para atualizar o parâmetro **Int** y Valor usado para atualizar o parâmetro |
| **void Substance.Game.SubstanceGraph**.*SetInputVector3Int*( string inputName, int x, int y, int z) | Atualizar Entrada Substance Vetor3Int | **Cadeia de caracteres** *inputName* Nome da entrada no SBSAR **Int** *x* Valor usado para atualizar o parâmetro **Int** y Valor usado para atualizar o parâmetro **Int** z Valor usado para atualizar o parâmetro |
| **int[] Substance.Game.SubstanceGraph**.*GetInputVector3Int*( string inputName) | Obter matriz de 3 int (valores x, y e z de Vetor3Int) | **Cadeia de caracteres** *inputName* Nome da entrada no SBSAR **Int** *x* Valor usado para atualizar o parâmetro **Int** y Valor usado para atualizar o parâmetro **Int** z Valor usado para atualizar o parâmetro |
| **void Substance.Game.SubstanceGraph**.*SetInputVector4Int*( string inputName, int x, int y, int z, int w) | Atualizar A Entrada Substance Vetor4Int | **Cadeia de caracteres** *inputName* Nome da entrada no SBSAR **Int** *x* Valor usado para atualizar o parâmetro **Int** y Valor usado para atualizar o parâmetro **Int** z Valor usado para atualizar o parâmetro **Int** w Valor usado para atualizar o parâmetro |
| **int[] Substance.Game.SubstanceGraph**.*GetInputVector4Int*( string inputName) | Obter matriz de 4 int (valores x, y, z &amp; w de Vetor4Int) | **Cadeia de caracteres** *inputName* Nome da entrada no SBSAR **Int** *x* Valor usado para atualizar o parâmetro **Int** y Valor usado para atualizar o parâmetro **Int** z Valor usado para atualizar o parâmetro **Int** w Valor usado para atualizar o parâmetro |
| **void Substance.Game.SubstanceGraph**.*SetInputString*(string inputName, valor de string) | Atualizar entrada da sequência de caracteres do Substance | **Cadeia de caracteres** *inputName* Nome da entrada no **valor** &lbrace;6 *do SBSAR usado para atualizar o parâmetro* |
| **Substance.Game.SubstanceGraph da cadeia de caracteres**.*GetInputString*( inputName da cadeia de caracteres) | Obter entrada de cadeia de caracteres de Substance | **Cadeia** *inputName* Nome da entrada no SBSAR |
| **void Substance.Game.SubstanceGraph**.*SetInputTexture*(string inputName, valor Textura2D) | Atualizar entrada Substance Textura2D | **Cadeia de caracteres** *inputName* Nome da entrada no **Textura2D** *valor* SBSAR usado para atualizar o parâmetro |
| **Substance.Game.SubstanceGraph** do Textura2D.*GetInputTexture*( inputName de cadeia de caracteres) | Obter entrada Substance Textura2D | **Cadeia** *inputName* Nome da entrada no SBSAR |
| **Substance VetorInt.Game.SubstanceGraph**.*GetTexturesResolution*() | Obtenha a resolução das texturas de Configurações de destino do gráfico (Vetor4Int’s x = width, y = height, values can be 32, 64, 128, 256, 512, 1024, 2048 &amp; 4096) | Nenh. |
| **int Substance.Game.SubstanceGraph**.*SetTexturesResolution*(tamanho de Vetor2Int) | Defina a resolução das texturas de Configurações de destino do gráfico (Vetor2Int’s x = width, y = height, values can be 32, 64, 128, 256, 512, 1024, 2048 &amp; 4096) Retorna 0 se bem-sucedido; caso contrário: -1. | **Vetor2Int** *size* usado para atualizar o parâmetro&#x200B;**.** |
| **Listar Substance.Game.SubstanceGraph**.*GetGeneratedTextures*() | Retorna todos os objetos Textura 2D de Substance usados pelo sombreador de material do gráfico. | Nenh. |
| **int Substance.Game.SubstanceGraph**.*Bake*(textura Texture2D, caminho absoluto da cadeia de caracteres) | Gere arquivos .png para todos os objetos Substance Textura2D usados pelo sombreador de material do gráfico. | Nenh. |
| **&#x200B;**&#x200B;Substance.Game.**&#x200B; SubstanceGraph**.*Duplicar*() | Duplicar um Gráfico do Substance | Nenh. |
| **Substance.Game.SubstanceGraph**.*Duplicar*(string newGraphName) | Duplique uma Gráfico do Substance e dê um nome a ela (o material correspondente também terá o mesmo nome) | **NewGraphName de cadeia de caracteres** |
| **&#x200B;**&#x200B;Substance.Game.**&#x200B; SubstanceGraph**.*GetInputProperties*() | Consultar informações de entrada de procedimento, retorna uma matriz de &#39;InputProperties&#39;, com :public struct InputProperties &lbrace; public string name; // inputName public string label; // o rótulo do widget no grupo público da string da GUI; // o grupo do widget na string pública da GUI[] componentLabels; // para controles deslizantes (até 4 rótulos) public string[] enumOptions; // para optionMenuplic InputPropertiesType type;public Vetor4 maximum; // para controles deslizantes públicos Vetor4 minimum; // para controles deslizantes public float step; // para controles deslizantes públicos enum InputPropertiesType { Boolean = 0,// 0 Float, // 1 Vetor2, // 2 Vetor3, // 3 Vetor4, // 4 Color, // 5 Enum, // 6 Texture, // 7 String, // 8 Invalid = -1// -1 }; | Nenh. |
| **bool** **Substance.Game.SubstanceGraph**.*HasInput*(**string** inputName) | Verificar se existe uma entrada em um gráfico retorna verdadeiro/falso: | **Cadeia** *inputName* Nome da entrada no SBSAR |
| **bool** **Substance.Game.SubstanceGraph**.*IsInputVisible*(**string** inputName) | Verificar se uma entrada visibleif está visível, retorna verdadeiro/falso | **Cadeia** *inputName* Nome da entrada no SBSAR |

## Renderização

| Método público | Descrição | Parâmetro |
| --- | --- | --- |
| public **void** *QueueForRender*() | Adicionar gráfico de Substance à fila | Nenh. |
| ***mySubstance.**&#x200B;RenderAsync()* | Renderizar todos os gráficos de Substance em fila de forma assíncrona | Nenh. |
| ***mySubstance.**&#x200B;RenderSync()* | Renderizar todos os gráficos de Substance em fila de forma síncrona | Nenh. |

## Script no modo Editor:

Para tornar as modificações do gráfico permanentes no modo Editor, uma reimportação de cada Substance correspondente deve ser executada. Isso é feito com a seguinte função:

```
static void ReImportSubstance(Substance.Game.Substance pSubstance)

{



// Re-import Substance object:

SubstanceImporter importer = AssetImporter.GetAtPath(pSubstance.assetPath) as SubstanceImporter;

importer.CommitSubstanceToImporter(pSubstance); // plugin function

EditorUtility.SetDirty(importer);

importer.SaveAndReimport();



}
```


(com “CommitSubstanceToImporter”, uma função de plug-in Substance: copie todos os parâmetros de gráfico modificados e/ou entradas para o objeto importador de Substance, que é então serializado em disco por meio do mecanismo importador do Unity)
