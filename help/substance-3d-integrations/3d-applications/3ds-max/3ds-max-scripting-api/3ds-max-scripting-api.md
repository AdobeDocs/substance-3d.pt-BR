---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/3ds-max/3ds-max-scripting-api.html"
breadcrumb-title: ''
description: Consulte a documentação da API de script do Substance 3ds Max para automatizar as operações de material.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds MAX Scripting API
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: API de script do 3ds MAX
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '895'
ht-degree: 2%

---


# API de script do 3ds MAX

Abaixo está a lista de comandos e propriedades para o nó Substance 2.

## Propriedades:

| Propriedade | Descrição | Tipo |
| --- | --- | --- |
| nome | Nome do Nó Substance2. O padrão é “Substance2” | String |

## Comandos:

| Comando | Descrição | Return | Tipo de retorno: | Parâmetro |
| --- | --- | --- | --- | --- |
| getCurrentPackageName | Obter o nome do arquivo base do pacote carregado (arquivo sbsar carregado no nó do gráfico) | O nome do arquivo (sem o diretório de prefixação) do pacote carregado (arquivo sbsar) | String |  |
| getCurrentGraphName | Obter o nome do gráfico atual | identificador da instância do gráfico atual | String |  |
| getOutputsNamesFromCurrentGraph | Obter a lista de nomes de uso de saída para saídas habilitadas | Tabela contendo lista de nomes de canais para saídas habilitadas | Lista |  |
| getPresetIdentifiers | Obter a lista de predefinições do gráfico de Substance | Tabela contendo a lista de identificadores de sequência de caracteres para todas as predefinições | Lista |  |
| setPackageAndGraphNames | Carregar um arquivo sbsar do disco no nó do gráfico | Verdadeiro no êxito, Falso no fracasso | Boolean | ***Parâmetro da cadeia de caracteres***: **substancePackageFilePath** O caminho para o arquivo sbsar no disco ***Parâmetro da cadeia de caracteres**: **graphInstanceNameToSelect** O identificador da cadeia de caracteres do gráfico |
| setInputInt | Definir uma entrada de inteiro com um novo valor |  |  | ***Parâmetro inteiro***: **valor** Valor inteiro para definir a entrada como ***parâmetro de cadeia de caracteres***: **inputIdentifier** O identificador de cadeia de caracteres exclusivo da entrada |
| setInputFloat | Definir uma entrada flutuante com um novo valor |  |  | ***Parâmetro de Precisão decimal***: **valor** Valor de Precisão decimal para definir a entrada como ***Parâmetro de cadeia de caracteres***: **inputIdentifier** O identificador de cadeia de caracteres exclusivo da entrada |
| setInputString | Definir uma entrada de cadeia de caracteres com um novo valor |  |  | ***Parâmetro de cadeia de caracteres***: **valor** Valor de cadeia de caracteres para definir a entrada como ***Parâmetro de cadeia de caracteres***: **identificadorDeEntrada** O identificador de cadeia de caracteres exclusivo da entrada |
| setInputBool | Definir uma entrada booleana com um novo valor |  |  | ***Parâmetro booliano:* valor &#x200B;** Valor booliano para definir a entrada como&#x200B;***Parâmetro de cadeia de caracteres &#x200B;***: **inputIdentifier** O identificador de cadeia de caracteres exclusivo da entrada |
| setInputVec2 | Definir uma entrada de vetor com dois elementos |  |  | ***Parâmetro Point2:**&#x200B;***valor** Valor máximo point2 para definir a entrada como ***Parâmetro de cadeia de caracteres &#x200B;***: **inputIdentifier** O identificador de cadeia de caracteres exclusivo da entrada |
| setInputVec3 | Definir uma entrada de vetor com três elementos |  |  | ***Parâmetro Point3:* valor &#x200B;** Valor máximo de point3 para definir a entrada como&#x200B;***Parâmetro de cadeia de caracteres &#x200B;***: **inputIdentifier** O identificador de cadeia de caracteres exclusivo da entrada |
| setInputVec4 | Definir uma entrada de vetor com quatro elementos |  |  | ***Parâmetro Point4***: **valor** Valor máximo de ponto4 para definir a entrada como ***parâmetro de cadeia de caracteres:* inputIdentifier &#x200B;** O identificador de cadeia de caracteres exclusivo da entrada |
| setInputColor | Definir uma entrada de cor com um novo valor |  |  | ***Parâmetro de cor***: **valor** Valor de cor máximo para definir a entrada como ***parâmetro de cadeia de caracteres:* inputIdentifier &#x200B;** O identificador de cadeia de caracteres exclusivo da entrada |
| setInputComboSelection | Definir o valor atualmente selecionado em uma entrada de caixa de combinação |  |  | ***Parâmetro inteiro***: **valor** Índice do widget de caixa de combinação ***Parâmetro de cadeia de caracteres***: **identificadorDeEntrada** O identificador de cadeia de caracteres exclusivo da entrada |
| getInputInt | Obter o valor de entrada para um tipo de entrada de inteiro | O valor inteiro atual da entrada | Integer | ***Parâmetro da cadeia de caracteres:* inputIdentifier &#x200B;** O identificador exclusivo da cadeia de caracteres da entrada |
| getInputFloat | Obter o valor de entrada para um tipo de entrada float | O valor de flutuação atual da entrada | Float | ***Parâmetro da cadeia de caracteres:* inputIdentifier &#x200B;** O identificador exclusivo da cadeia de caracteres da entrada |
| getInputString | Obter o valor de entrada para um tipo de entrada de cadeia de caracteres | O valor da cadeia de caracteres atual da entrada | String | ***Parâmetro da cadeia de caracteres:* inputIdentifier &#x200B;** O identificador exclusivo da cadeia de caracteres da entrada |
| getInputBool | Obter o valor de entrada para um tipo de entrada booleano | O valor booleano atual da entrada | Boolean | ***Parâmetro da cadeia de caracteres:* inputIdentifier &#x200B;** O identificador exclusivo da cadeia de caracteres da entrada |
| getInputVec2 | Obter o valor de entrada para um tipo de entrada point2 | O valor de ponto2 máximo atual da entrada | Ponto2 | ***Parâmetro da cadeia de caracteres:* inputIdentifier &#x200B;** O identificador exclusivo da cadeia de caracteres da entrada |
| getInputVec3 | Obter o valor de entrada para um tipo de entrada point3 | O valor de ponto3 máximo atual da entrada | Ponto3 | ***Parâmetro da cadeia de caracteres:* inputIdentifier &#x200B;** O identificador exclusivo da cadeia de caracteres da entrada |
| getInputVec4 | Obter o valor de entrada para um tipo de entrada point4 | O valor de ponto máximo 4 atual da entrada | Ponto4 | ***Parâmetro da cadeia de caracteres:* inputIdentifier &#x200B;** O identificador exclusivo da cadeia de caracteres da entrada |
| getInputColor | Obter o valor de entrada para um tipo de entrada de cor | O valor atual da entrada como uma cor | Cor | ***Parâmetro da cadeia de caracteres:* inputIdentifier &#x200B;** O identificador exclusivo da cadeia de caracteres da entrada |
| getInputComboSelection | Obtém o índice da seleção da caixa de combinação com base no identificador | O índice do item da caixa de combinação selecionado | Integer | ***Parâmetro da cadeia de caracteres:* inputIdentifier &#x200B;** O identificador exclusivo da cadeia de caracteres da entrada |
| getMaterialDependentCount | Obter o número de dependências de material | O número de referências dependentes de um tipo de material | Integer |  |
| AplicarValoresParaPredefiniçãoSelecionada | Substitui a predefinição atualmente selecionada pelos valores de entrada atuais |  |  |  |
| RemoveAllPresets | Remover todas as predefinições no nó do gráfico atual |  |  |  |
| CreatePreset | Criar uma nova predefinição a partir das entradas atuais |  |  | ***Parâmetro da cadeia de caracteres:* newPresetName &#x200B;** Nome para exibição da nova predefinição |
| RemoverUmaPredefinição | Remover a predefinição com o nome fornecido |  |  | ***Parâmetro da cadeia de caracteres:* seletedPresetName &#x200B;** Nome da predefinição a ser removida |
| ImportPreset | Importar o arquivo sbsprs para as predefinições atuais |  |  | ***Parâmetro da cadeia de caracteres:**&#x200B;***filePath** Cadeia de caracteres contendo o caminho do arquivo do qual importar a predefinição |
| ExportPreset&#x200B;**\*deprecated** Para remover na versão 2.5.0\* | Exportar a predefinição atualmente selecionada para um arquivo sbsprs |  |  | ***Parâmetro da cadeia de caracteres***: **filePath** cadeia de caracteres contendo o caminho do arquivo para o qual exportar a predefinição |
| exportPresetList | Exportar as predefinições fornecidas para um único arquivo de predefinição |  |  | ***Parâmetro de cadeia de caracteres***: **filePath** cadeia de caracteres contendo o caminho do arquivo para exportar as predefinições para ***Parâmetro de lista***: **predefinições** lista contendo os nomes das predefinições a serem exportadas |
| CozinharSaídasDoGráficoSelecionado | Transferir os bitmaps da instância de gráfico selecionada para o disco |  |  | ***Parâmetro de cadeia de caracteres:* filePath &#x200B;** O diretório de caminho raiz no qual gravar as imagens é inserido&#x200B;***Parâmetro de cadeia de caracteres &#x200B;***: **imageFormatExtension** A extensão/formato de arquivo no qual gravar as imagens |
