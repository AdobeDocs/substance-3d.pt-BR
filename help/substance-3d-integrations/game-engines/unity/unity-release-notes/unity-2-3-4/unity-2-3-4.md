---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-3-4.html"
breadcrumb-title: ''
description: Consulte as notas de versão do plug-in Unity versão 2.3.4 para saber mais sobre novos recursos, aprimoramentos e correções de erros.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.3.4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.3.4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%

---


# Unity 2.3.4

>[!WARNING]
>
> **Usar o plug-in com o Unity 2019.2 produzirá o seguinte erro:**
> 
> InspectorSubstanceImporter.OnInspectorGUI deve chamar ApplyRevertGUI para evitar comportamento inesperado.\
> UnityEditor.Experimental.AssetImporters.AssetImporterEditor:OnDisable()\
> Substance.Editor.InspectorSubstanceImporter:OnDisable()
> 
> Este erro pode ser apagado e não afetará a funcionalidade do plug-in

>[!WARNING]
>
> **Leia: quebra de materiais de Substance:**\
> Os materiais de Substance que contêm uma saída personalizada com um uso em branco serão interrompidos na importação. Além disso, os materiais de Substance que contêm usos duplicados serão quebrados.\
> Arquivos sbsar mais antigos do GameTextures.com não são compatíveis atualmente com o plug-in Substance no Unity. Esses materiais que contêm saídas de Uso sem suporte estão sendo interrompidos. Antes de usar o plug-in, certifique-se de fazer um backup do projeto.

## Novos recursos:

* Suporte adicionado para Substance Engine v7
* Adicionado suporte a Linux

### Correções de erros:

* Corrigidos problemas relacionados à importação de um Substance sem nenhum mapa de textura
* Correção de um problema com o processo de reflexão que não funcionava corretamente no Unity 2019.x
* Correção de problemas de manuseio pré-fabricado ao importar um pacote contendo pré-fabricações com materiais Substance
* Atribuições fixas de material/textura não transitadas após o processo de reflexão
* Correção de um problema relacionado à alteração de sombreadores que causava quebra de materiais
* Correção de um problema em que a aspereza não era embalada no canal alfa metálico
* Correção de um problema em que, quando o plug-in Substance era instalado, a alteração das configurações de importação para texturas que não são da substância revertia determinadas opções.
* Correção de um problema em que o Substance Source não abria no Mac

## Problemas conhecidos:

**Plug-in Core Substance**

* O usuário deve desativar &#39;Ativar Bitcode&#39; no menu Configurações de Compilação no Xcode para compilar para o iOS
* Os Substance não funcionam com pacotes de ativos
* Todos os ícones de visualização de Substance no Navegador de ativos mudam para o ícone Substance S após uma reimportação
* Os materiais de Substance personalizados que têm uma saída com uso definido como em branco quebrarão o material
* Os materiais de Substance personalizados que têm usos duplicados quebrarão o material
* O Editor deve ser reiniciado após a importação do plug-in no Linux

**Script**

* O script não funciona em tempo de execução se o projeto estiver definido como x86 nas configurações de compilação
* Problemas ao usar o backend de script il2cpp com determinadas plataformas de compilação

**Live Link do Substance Painter**

* Criar um projeto após pintar com o Substance Live Link definirá a malha pintada de volta para um material padrão
* Canal AO não enviado com o link do Painter Live
* Malhas com vários materiais não funcionam no Unity Live Link
* A forma como o Unity LiveLink usa o SimpleJson entra em conflito com outras instâncias do SimpleJson em um projeto
