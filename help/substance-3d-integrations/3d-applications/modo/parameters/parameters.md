---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/modo/parameters.html"
breadcrumb-title: ''
description: Modifique os parâmetros de material de Substance em MODO através do painel Propriedades do Substance para personalizar materiais.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > MODO > Parameters
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Parâmetros
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---


# Parâmetros

Um Substance tem um conjunto de parâmetros principais. Esses parâmetros são divididos em Substance, Saídas e Ajustes. Eles podem ser encontrados no painel Propriedades do Substance.\
O Substance de Substance Source conterá Parâmetros Técnicos e Canais. As opções de Canal não têm efeito no MODO. As saídas são ativadas/desativadas usando a seção Saídas.

![](../../../assets/parameters-4.png){width="300px"}

## de substâncias

Um Substance tem um conjunto de parâmetros principais, que podem ser encontrados na categoria Substance do painel Propriedades do Substance.

* **Recarregar Substance:** este parâmetro permite recarregar um Substance. Foi projetado para uso com o Substance Designer. Se você estiver trabalhando em um Substance personalizado e tiver adicionado um novo ajuste ou saída, poderá recarregar o Substance recém-publicado de volta no MODO. Os novos ajustes e saídas serão adicionados e as configurações de ajuste anteriores permanecerão.
* **Modo de Sombreamento:** este parâmetro permite que você defina o modo de sombreamento a ser usado para o Substance. Princípio (padrão), Irreal, Unity ou glTF.
* **Redefinir Substance:** este parâmetro redefinirá os ajustes para as configurações padrão.
* **Selecionar gráfico:** permite que você escolha qual gráfico no arquivo de Substance a partir do qual um material será criado.
* **Carregar predefinição:** você pode carregar uma predefinição, que configurará os parâmetros de ajuste de Substance. As predefinições podem ser criadas usando Substance Player. O arquivo de predefinição é um tipo de arquivo .sbsprs. Depois de carregar uma predefinição, você precisa clicar no menu suspenso Predefinição e escolher a predefinição, pois um arquivo .sbsprs pode conter várias predefinições.
* **Salvar predefinição:** permite salvar uma predefinição
* **Selecionar predefinição:** permite escolher uma predefinição incorporada no arquivo de Substance ou entre as predefinições salvas dentro do MODO.
* **Fazer bake em Disco:** este parâmetro fará bake as textura geradas pelo Substance em um arquivo de bitmap.
* **Tamanho de Saída:** este parâmetro redimensionará dinamicamente a textura para o tamanho definido. O Substance Engine regenerará a textura para o tamanho desejado.
* **Distribuição aleatória:** este parâmetro variará a geração processual do Substance. Esse parâmetro é ótimo para criar uma versão aleatória do mesmo Substance. Ele permite que você varie rapidamente os parâmetros de Substance para gerar uma nova versão do textura

## Saídas

As opções de Saída permitem ativar ou desativar as saídas de Substance. Uma saída é o que é gerado pelo Substance Engine e renderizado como uma textura na Árvore de Sombreadores.

![](../../../assets/outputs-02.png){width="300px"}

## Ajustes

Ajustes são parâmetros criados no arquivo Substance e editáveis no MODO. Você pode selecionar canais e, no Modo de item, usar o Haul de canal para reunir os controles em um controlador pop-up.

![](../../../assets/haul.png){width="300px"}
