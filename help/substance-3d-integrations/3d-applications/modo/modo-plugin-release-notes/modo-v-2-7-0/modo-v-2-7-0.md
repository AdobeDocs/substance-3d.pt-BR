---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/modo/modo-plugin-release-notes/modo-v-2-7-0.html"
breadcrumb-title: ''
description: Consulte as notas de versão do plug-in MODO versão 2.7.0 para saber mais sobre novos recursos, melhorias e correções de erros.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Modo Plugin Release Notes > Modo v. 2.7.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Modo v. 2.7.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---


# Modo v. 2.7.0

* Várias correções de falhas
* Suporte a float de 32 bits
* Texturas de 4k no mecanismo da CPU e texturas de 8k no mecanismo da GPU
* novo formato LPK para a versão de plug-in
* novo menu do Kit para o plug-in Substance
* Suporte a glTF/Principled Shader para MODO 12.0
* Caminho relativo adicionado para arquivos Substance
* Suporte a Linux
* Nova interface para carregar e salvar predefinições
* As predefinições incorporadas são carregadas do Designer
* Caixa de aviso Memória GPU removida
* Comandos de carregamento/salvamento de predefinições editados

  Os novos comandos disponíveis são:

  **substance.getsbsname** converte o identificador de um objeto substance em seu nome interno

  Todos eles esperam um nome interno adequado adquirido de substance.getsbsname:

  **substance.setpreset** Define uma predefinição atual de Substance para o índice **substance.getpresetindex** Obtém o índice de predefinição atual **substance.getpresetat** Retorna o nome da cadeia de caracteres de uma predefinição em um determinado **index substance.getpresetcount** Retorna o número de predefinições que um Substance tem **substance.savepresetfile** Salva uma predefinição da configuração atual para o caminho de arquivo especificado **substance.loadpresetfile** Carrega um arquivo de predefinição ao Substance dado um caminho de arquivo

  Comandos de interface:

  Comando de interface do usuário do **substance.loadpresetui** para carregar um comando de interface do usuário predefinido **substance.savepresetui** para salvar um comando de interface do usuário predefinido **substance.selectpresetui** para definir a predefinição
