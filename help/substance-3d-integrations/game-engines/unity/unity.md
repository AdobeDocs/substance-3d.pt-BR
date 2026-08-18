---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/game-engines/unity.html"
breadcrumb-title: ''
description: Importe e use materiais de Substance no mecanismo de jogo do Unity com suporte nativo a plug-ins e controle de parâmetros de tempo de execução.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Unidade
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '743'
ht-degree: 0%

---


# Unidade

![](../../assets/unity.png)

>[!NOTE]
>
> **Versões com Suporte do Unity**
> 
> O plug-in Adobe Substance 3D para Unity versão 3.0.0 atualmente oferece suporte ao Unity 2020.3.27x e superior. Ele pode ser baixado do [Repositório de Ativos do Unity](https://assetstore.unity.com/packages/tools/utilities/substance-3d-for-unity-beta-213208).

>[!WARNING]
>
> Antes de atualizar ou usar o plug-in, verifique a [página de atualização do projeto](https://helpx.adobe.com/br/substance-3d/unlisted/documentation/integrations/upgrading-projects-182256244.html).

>[!WARNING]
>
> Verifique a página [Diretrizes de Otimização](../../game-engines/unity/optimization-guidelines/optimization-guidelines.md) antes de criar materiais de Substance personalizados.

## Sumário

* [Notas de versão do Unity](https://helpx.adobe.com/br/substance-3d/unlisted/documentation/integrations/beta-release-information-170460277.html) — Novidades do plug-in Substance in Unity por versão
* [Baixando o plug-in Substance 3D no Unity](../../game-engines/unity/downloading-plugin-unity/downloading-substance-3d-plugin-in-unity.md) — o Adobe Substance 3D para Unity está disponível no Unity Asset Store https://assetstore.unity.com/packages/tools/utilities/substance-in-unity-110555.
* [Visão geral do plug-in Unity](../../game-engines/unity/unity-plugin-overview/unity-plugin-overview.md)
* [Preferências do Unity](../../game-engines/unity/unity-preferences/unity-preferences.md) — A janela de preferência do Substance permite que você defina opções definidas pelo usuário para o plug-in.
* [Diretrizes de otimização](../../game-engines/unity/optimization-guidelines/optimization-guidelines.md) — ao criar seus próprios materiais de Substance personalizados, verifique as seguintes diretrizes de otimização.
* [Atualizando projetos/problemas conhecidos](https://helpx.adobe.com/br/substance-3d/unlisted/documentation/integrations/upgrading-projects-182256244.html) — problemas conhecidos com o Substance no plug-in Unity
* [Gerenciando Gráficos do Substance](https://helpx.adobe.com/br/substance-3d/unlisted/documentation/integrations/managing-and-navigating-substance-graphs-170459636.html) — você pode criar novos materiais com base no material do Substance usando o SGM (Gerenciador de Gráficos do Substance)
* [Alterando parâmetros](../../game-engines/unity/changing-parameters/changing-parameters.md) — Parâmetros para o material de Substance estão acessíveis no SGO (Objeto de Gráfico do Substance).
* [Texturas Geradas (Embalagem)](../../game-engines/unity/generated-textures-pac/generated-textures-packing.md) — As Texturas Geradas mostram as saídas do Substance que são computadas pelo Substance Engine para criar texturas
* [Espaço da cor de renderização](../../game-engines/unity/rendering-color-space/rendering-color-space.md) — para obter os melhores resultados, você deve definir o espaço da cor como linear nas Configurações do Reprodutor de Unidade.
* [Utilização de entradas de imagem](../../game-engines/unity/using-image-inputs/using-image-inputs.md)
* [Publicação para dispositivos móveis](../../game-engines/unity/publishing-for-mobile/publishing-for-mobile.md) — Diretrizes para publicação em plataformas móveis
* [Substance 3D para Script de Unidade](../../game-engines/unity/3d-for-unity-scripting/substance-3d-for-unity-scripting.md) — Usando a API Substance, você pode gravar scripts para atualizar e alterar parâmetros de Substance em tempo de execução.
* [Scripts no Unity (Preterido)](https://helpx.adobe.com/br/substance-3d/unlisted/documentation/integrations/scripting-in-unity-170459644.html) — Usando a API Substance, você pode gravar scripts para atualizar e alterar parâmetros de Substance no tempo de execução.
* [Uso da Biblioteca do Substance 3D Assets](https://helpx.adobe.com/br/substance-3d/unlisted/documentation/integrations/substance-3d-assets-library-225970070.html)
* [Removendo plug-in Substance](../../game-engines/unity/removing-plugin/removing-substance-plugin.md)
* [Substance 3D no Unity Tutorials](../../game-engines/unity/3d-in-unity-tutorials/substance-3d-in-unity-tutorials.md)
* [Tamanho físico no Unity](../../game-engines/unity/physical-size-in-unity/physical-size-in-unity.md)
* [Compartilhando Arquivos Sbsar Entre Projetos](https://helpx.adobe.com/sharing-sbsar-files-between-projects.html) [&#128279;](../../game-engines/unity/sharing-sbsar-files-bet/sharing-sbsar-files-between-projects.md)

**[FORMULÁRIO ENCONTRADO - REGRAS NECESSÁRIAS]**

>[!WARNING]
>
> Antes de atualizar ou usar o plug-in, verifique a [página de atualização do projeto](https://helpx.adobe.com/br/substance-3d/unlisted/documentation/integrations/upgrading-projects-182256244.html).

>[!WARNING]
>
> Verifique a página [Diretrizes de Otimização](../../game-engines/unity/optimization-guidelines/optimization-guidelines.md) antes de criar materiais de Substance personalizados.

### Sumário

* [Notas de versão do Unity](https://helpx.adobe.com/br/substance-3d/unlisted/documentation/integrations/beta-release-information-170460277.html) — Novidades do plug-in Substance in Unity por versão
* [Baixando o plug-in Substance 3D no Unity](../../game-engines/unity/downloading-plugin-unity/downloading-substance-3d-plugin-in-unity.md) — o Adobe Substance 3D para Unity está disponível no Unity Asset Store https://assetstore.unity.com/packages/tools/utilities/substance-in-unity-110555.
* [Visão geral do plug-in Unity](../../game-engines/unity/unity-plugin-overview/unity-plugin-overview.md)
* [Preferências do Unity](../../game-engines/unity/unity-preferences/unity-preferences.md) — A janela de preferência do Substance permite que você defina opções definidas pelo usuário para o plug-in.
* [Diretrizes de otimização](../../game-engines/unity/optimization-guidelines/optimization-guidelines.md) — ao criar seus próprios materiais de Substance personalizados, verifique as seguintes diretrizes de otimização.
* [Atualizando projetos/problemas conhecidos](https://helpx.adobe.com/br/substance-3d/unlisted/documentation/integrations/upgrading-projects-182256244.html) — problemas conhecidos com o Substance no plug-in Unity
* [Gerenciando Gráficos do Substance](https://helpx.adobe.com/br/substance-3d/unlisted/documentation/integrations/managing-and-navigating-substance-graphs-170459636.html) — você pode criar novos materiais com base no material do Substance usando o SGM (Gerenciador de Gráficos do Substance)
* [Alterando parâmetros](../../game-engines/unity/changing-parameters/changing-parameters.md) — Parâmetros para o material de Substance estão acessíveis no SGO (Objeto de Gráfico do Substance).
* [Texturas Geradas (Embalagem)](../../game-engines/unity/generated-textures-pac/generated-textures-packing.md) — As Texturas Geradas mostram as saídas do Substance que são computadas pelo Substance Engine para criar texturas
* [Espaço da cor de renderização](../../game-engines/unity/rendering-color-space/rendering-color-space.md) — para obter os melhores resultados, você deve definir o espaço da cor como linear nas Configurações do Reprodutor de Unidade.
* [Utilização de entradas de imagem](../../game-engines/unity/using-image-inputs/using-image-inputs.md)
* [Publicação para dispositivos móveis](../../game-engines/unity/publishing-for-mobile/publishing-for-mobile.md) — Diretrizes para publicação em plataformas móveis
* [Substance 3D para Script de Unidade](../../game-engines/unity/3d-for-unity-scripting/substance-3d-for-unity-scripting.md) — Usando a API Substance, você pode gravar scripts para atualizar e alterar parâmetros de Substance em tempo de execução.
* [Scripts no Unity (Preterido)](https://helpx.adobe.com/br/substance-3d/unlisted/documentation/integrations/scripting-in-unity-170459644.html) — Usando a API Substance, você pode gravar scripts para atualizar e alterar parâmetros de Substance no tempo de execução.
* [Uso da Biblioteca do Substance 3D Assets](https://helpx.adobe.com/br/substance-3d/unlisted/documentation/integrations/substance-3d-assets-library-225970070.html)
* [Removendo plug-in Substance](../../game-engines/unity/removing-plugin/removing-substance-plugin.md)
* [Substance 3D no Unity Tutorials](../../game-engines/unity/3d-in-unity-tutorials/substance-3d-in-unity-tutorials.md)
* [Tamanho físico no Unity](../../game-engines/unity/physical-size-in-unity/physical-size-in-unity.md)
