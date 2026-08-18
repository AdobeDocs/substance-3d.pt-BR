---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-5/installing-to-source-builds-ue5.html"
breadcrumb-title: ''
description: Instale o plug-in do Substance 3D nas compilações de origem do Unreal Engine 5 para modificações personalizadas do mecanismo.
helpx_creative_field: ""
helpx_description: Substance 3D Integrations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Instalando em compilações de origem - UE5
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '303'
ht-degree: 0%

---


# Instalando em compilações de origem - UE5

O plug-in Substance pode ser usado com versões do Unreal Engine construído a partir da fonte. Para fazer isso, o plug-in pode ser instalado em uma pasta do projeto C++ ou na pasta do mecanismo de uma compilação de código-fonte.

>[!NOTE]
>
> Esses métodos exigem que você tenha uma versão do plug-in baixada do marketplace. A pasta de plug-ins Substance pode ser transferida entre computadores e compilações UE.

## Instalando em uma pasta do projeto C++

1. Na pasta do projeto, crie uma pasta Plug-ins se ainda não existir uma.
1. Dentro da pasta Plugins, crie uma pasta Runtime.
1. Coloque a pasta Substance dentro da pasta Runtime. USUÁRIOS DO LINUX: após a etapa 3, localize a pasta “include” na pasta Substance e renomeie-a para colocar em maiúsculas o “i” (include > Include).
1. Inicie o Unreal Engine.
1. Abra o projeto C++ através do iniciador.
1. Depois de iniciar o projeto, Unreal Engine perguntará se você gostaria de reconstruir componentes de plug-in antes de iniciar, selecione sim. Isso será feito por meio do Microsoft Visual Studio (Windows, Linux) ou do Xcode (Mac).
1. Unreal Engine será fechado, mas os componentes serão criados em segundo plano. Esse processo pode levar cerca de 5 minutos. Depois de concluído, o projeto será aberto. Se falhar, você verá uma janela de erro.

## Instalando na pasta Engine

>[!NOTE]
>
> As etapas acima devem ser seguidas para recriar a pasta Binaries do plug-in antes que o plug-in possa ser instalado na pasta Engine.

1. Copie a pasta Substance de dentro da Pasta do projeto > Plug-ins > Tempo de execução.
1. Abra a pasta da versão do Unreal Engine e navegue até Mecanismo > Plug-ins > Marketplace.
1. Cole a pasta Substance.
1. Abra o Unreal Engine Editor. Crie um novo projeto, se desejar.
1. Abra o menu Plug-ins e verifique se o plug-in Substance está ativado.
