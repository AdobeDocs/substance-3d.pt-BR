---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/maya/settings.html"
breadcrumb-title: ''
description: Defina as configurações do plug-in de Substance no Maya por meio da prateleira ou menu de Substance para personalizar o comportamento.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Maya > Settings
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Configurações
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 1%

---


# Configurações

O menu de configurações de Substance pode ser acessado através do Substance Shelf ou do menu Substance. As configurações desse menu são armazenadas em um arquivo de configuração editável “substance.cfg”.

>[!NOTE]
>
> **Locais dos Arquivos de Configuração**
> 
> **Windows**:\
> C:\Users\\Documents\maya\\substance\\
> **MacOS**:\
> /Users//Library/Preferences/Autodesk/maya//substance/\
> **Linux**:\
> /home//maya//substance/

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

## Resolução padrão

Define a resolução padrão de um nó Substance quando o arquivo sbsar é carregado.

## Fluxo de trabalho de renderização

Define o fluxo de trabalho de renderização padrão a ser usado no nó Substance.

## Substance Engine

Definindo preferências específicas para o Substance Engine e globais para todos os nós de Substance. O mecanismo de Substance é usado para calcular as texturas de Substance.

### Tipo de mecanismo

O Substance Engine está disponível como um mecanismo de CPU e GPU. Alternar o mecanismo exigirá a reinicialização do Maya. O mecanismo da GPU permitirá resoluções mais altas do que o mecanismo da CPU.

>[!WARNING]
>
> Pode haver diferenças de cálculo entre a CPU e o mecanismo da GPU. Portanto, para resultados consistentes, é melhor definir o tipo para o mesmo mecanismo usado no Substance Designer.

Os núcleos da CPU e a memória do mecanismo são configurações para a quantidade de recursos que o mecanismo de Substance pode usar.

### Bloqueando renderizações

Esta opção permite definir se o computador do mecanismo de Substance bloqueará os processos de interface do Maya. Quando ativado, o mecanismo Substance terá precedência e bloqueará os processos de interface do Maya. Quando desabilitados, os processos de interface do Maya não serão bloqueados por cálculos do mecanismo Substance.

## Saídas do cache para o disco

Define o local de cache padrão, o tipo de arquivo e a pasta de cache para todos os nós de Substance recém-criados em um projeto.

## Renderizando extensões

Ative as extensões de renderização para usar saídas de Substance diretamente com Arnold Shaders.

## Tamanho físico

Habilite se o Tamanho físico deve ser usado por padrão quando os arquivos sbsar são carregados e se deve ser recalculado ao recarregar o sbsar.

</td>
<td style="border: 0;" valign="top">

![](../../../assets/settings-35.png)

</td>
</tr>
</table>
