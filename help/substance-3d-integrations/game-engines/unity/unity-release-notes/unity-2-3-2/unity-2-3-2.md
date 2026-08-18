---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/game-engines/unity/unity-release-notes/unity-2-3-2.html"
breadcrumb-title: ''
description: Consulte as notas de versão do plug-in Unity versão 2.3.2 para saber mais sobre novos recursos, aprimoramentos e correções de erros.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Unity Release Notes > Unity 2.3.2
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unity 2.3.2
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---


# Unity 2.3.2

## Novos recursos:

* Serialização de material
* Reflexo: O plugin agora permite a importação de arquivos Substance antigos em pacotes (automaticamente atualizado para novos dados Substance na importação)
* As propriedades dos materiais são mantidas na importação de pacotes com dados de Substance
  * Observação: isso se aplica somente a pacotes criados usando a atualização 2.3.0 ou posterior
* Adicionado o botão Textura do bolo ao menu de gráfico de Substance

### Correções de erros:

* Correção de um problema em que a divisão de material do Substance era redefinida se a pasta Biblioteca fosse removida
* Velocidade aprimorada ao sair do modo de reprodução
* Correção de uma falha ao atualizar o plug-in enquanto a DLL de Substance estava em uso
* A pasta Allegorithmic agora não pode ser excluída dentro do Unity.
  * Observação: o conteúdo da pasta Allegorithmic não pode ser modificado. Excluí-lo dentro do Unity pode causar vários problemas, fazendo com que a pasta Allegorithmic reapareça magicamente quando o Unity é fechado e reaberto. Agora há um aviso que informa ao usuário para excluí-lo com o Unity fechado manualmente na pasta Ativos do projeto
* Velocidade aprimorada ao sair do modo de reprodução
* Correção de um erro que redefinia as propriedades do material do Substance quando a pasta Biblioteca era removida

## Problemas conhecidos:

**Plug-in Core Substance**

* O usuário deve desativar &#39;Ativar Bitcode&#39; no menu Configurações de Compilação no Xcode para compilar para o iOS
* Os Substance não funcionam com pacotes de ativos
* Todos os ícones de visualização de Substance no Navegador de ativos mudam para o ícone Substance S após uma reimportação

**Script**

* O script não funciona em tempo de execução se o projeto estiver definido como x86 nas configurações de compilação
* Problemas ao usar o backend de script il2cpp com determinadas plataformas de compilação

**Live Link do Substance Painter**

* Criar um projeto após pintar com o Substance Live Link definirá a malha pintada de volta para um material padrão
* Canal AO não enviado com o link do Painter Live
* Malhas com vários materiais não funcionam no Unity Live Link
* A forma como o Unity LiveLink usa o SimpleJson entra em conflito com outras instâncias do SimpleJson em um projeto
