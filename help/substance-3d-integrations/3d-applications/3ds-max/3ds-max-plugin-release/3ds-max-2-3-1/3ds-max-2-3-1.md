---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/3d-applications/3ds-max/3ds-max-plugin-release-notes/3ds-max-2-3-1.html"
breadcrumb-title: ''
description: Consulte as notas de versão do plug-in 3ds Max versão 2.3.1 para saber mais sobre novos recursos, melhorias e correções de erros.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > 3ds Max > 3ds Max Plugin Release Notes > 3ds Max 2.3.1
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: 3ds Max 2.3.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---


# 3ds Max 2.3.1

Lançado em 13 de fevereiro de 2020

O plug-in agora é instalado fora do diretório do 3ds Max em C:\ProgramData\Autodesk\ApplicationPlugins\SubstanceIn3dsMax. Ele agora deve funcionar em qualquer lugar que o 3ds Max é instruído a procurar plug-ins, de modo que agora deve funcionar instalado em uma unidade de rede, etc.\
Observe que a alternância entre o Plug-in de aplicativo e o diretório de instalação faz com que uma atualização das versões 2.1.1 e anteriores não funcione corretamente. Eles devem ser removidos manualmente para o 3ds Max 2018 e 2019. A versão 2.2.0 deve ser atualizada corretamente.\
Para alguns dos problemas não solucionados nesta versão, há outro planejado para corrigir em breve esses e outros problemas que possam surgir.

Esta versão é lançada atualmente para o 3ds Max 2018, 2019, 2020 e 2021.

* Carregar sbsar agora procura na pasta de imagens do projeto primeiro
* A caixa de diálogo de compatibilidade do renderizador agora aparece somente para o Renderizador VRay RT e VUE File
* Arrastar e soltar para o Editor de material de ardósia desativado para remover problemas com o lote Máximo
* A caixa de diálogo Renderizar não é mais exibida no modo silencioso do 3ds Max
* Os scripts Python menores agora são compatíveis com o Python 3
* Foi adicionado suporte ao Substance Launcher para enviar ativos de Substance Source para o 3ds Max. Isso exigirá alterações no Iniciador, mas haverá suporte no plug-in à medida que o recurso for adicionado.
* O script do renderizador Redshift agora usa os novos nomes de nó definidos no Redshift 2.6.24
* Max não trava mais quando um caminho vazio é atribuído a Substance2 SubstanceFilePath
* Remova a colisão de nomes do tipo SubstanceOutput com o plug-in antigo
* Classe SubstanceOutput renomeada para Substance2Output
* Classe do Gerenciador de menus do Substance renomeada para Substance2MenuManager
* Os IDs de blocos de parâmetros agora são limpos de modo forçado quando uma cena é aberta, removendo colisões entre arquivos de cena. Isso deve corrigir problemas com blocos de parâmetro inválidos no carregamento ao alternar entre cenas. A importação ainda pode ter problemas, pois isso requer alterações mais complexas
* O plug-in agora está instalado fora do 3ds Max. Todos os caminhos foram alterados para relativos a partir do local de carregamento.
* O plug-in agora usa o sistema de plug-ins Autodesk Application.
