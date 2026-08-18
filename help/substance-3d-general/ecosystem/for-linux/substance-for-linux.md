---
helpx_url: "https://helpx.adobe.com/br/substance-3d-general/ecosystem/substance-for-linux.html"
breadcrumb-title: ''
description: Saiba como baixar, instalar e ativar os aplicativos da Substance 3D no Linux usando o portal Adobe Download Access.
helpx_creative_field: ""
helpx_description: Substance 3D General
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Substance 3D para Linux (ADA)
user-guide-description: ''
user-guide-title: ''
source-git-commit: 081136918fdf7f431ecee47e5ce64d8b5235bb1b
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---


# Guia de implantação

Após adquirir o Substance 3D para Linux® por meio de seu contrato Enterprise, os produtos e licenças correspondentes serão provisionados no portal [Adobe Download Access (ADA)](https://download-access.adobe.com/lws/downloads). Você precisará baixar os builds do software e os arquivos da chave de licença do ADA para implantar o software com êxito.

## Baixar versões de software e arquivos de chave de licença:

Entre no [Acesso para Download do Adobe](https://download-access.adobe.com/lws/downloads). Encontre os builds do software e os arquivos da chave de licença:

1. Use o menu suspenso Conta para selecionar a conta na qual você adquiriu o Substance 3D Linux.

   ![](../../assets/ADA1.png)
1. Navegue até Downloads com o link no cabeçalho da página.

   ![](../../assets/ADA2.png)
1. Clique em Ver downloads no produto correspondente.

   ![](../../assets/ADA3.png)
1. O ADA carregará as informações de licença associadas a essa ID e as exibirá na tabela abaixo.
1. Clique em “Download” na linha “Certificado digital” para baixar o arquivo zip que contém os arquivos de chave de licença.

   * O arquivo zip contém uma chave de licença por produto.
   * A chave de licença ativará o produto em cada um dos computadores licenciados.

   ![](../../assets/ADA4.png)
1. Clique em “Substance 3D”, Sampler, Painter ou Designer para exibir as compilações de software do Substance 3D Painter, Substance 3D Designer e Substance 3D Sampler.
1. Clique em “Download” para baixar o arquivo de instalação do produto que deseja instalar.

   ![](../../assets/ADA5.png)
1. Será exibida uma notificação “Download de software”. Clique em “aceitar”

   ![](../../assets/ADA6.png)

## Instalação e ativação

Para instalar o software:

1. Clique duas vezes no arquivo EXE do produto para iniciar o assistente de instalação.
1. Siga as etapas de instalação para concluir a instalação.

Há duas opções para a ativação do software: ativação local ou ativação de rede.

### Ativação local

1. Descompacte a pasta zip baixada do ADA.
1. Inicie o software que deseja ativar.
1. No assistente de ativação, selecione “Ativar usando um arquivo de chave de licença”.

   ![](../../assets/LinuxActivation3.png)
1. Clique em “Procurar” e aponte para o local do arquivo de chave de licença correspondente.
1. Clique em “Avançar” para ativar o software.

### Ativação de rede

1. Descompacte a pasta zip baixada do ADA.
1. Coloque os arquivos de chave de licença descompactados em uma rede montada compartilhada.
1. No computador do usuário, configure uma variável de ambiente que aponte para o arquivo de chave de licença conforme explicado nestas páginas:

   * Substance 3D Painter - <https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/pipeline-and-integration/configuration/environment-variables>
   * Substance 3D Designer - <https://experienceleague.adobe.com/en/docs/substance-3d-designer/using/pipeline-and-project-configuration/environment-variables>
   * Substance 3D Sampler - <https://experienceleague.adobe.com/en/docs/substance-3d-sampler/using/pipeline-and-integrations/environment-variables>
