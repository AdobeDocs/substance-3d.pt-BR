---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/3d-applications/blender/release-notes/add-on-0-9-1.html"
breadcrumb-title: ''
description: Consulte as notas de versão do complemento do Blender versão 0.9.1 para saber mais sobre novos recursos, aprimoramentos e correções de erros.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > Release Notes > Add-on 0.9.1
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Complemento 0.9.1
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 0%

---


# Complemento 0.9.1

**Notas de versão do Complemento versão 0.91+**

* Observação: *A versão 0.91+ do plug-in não tem compatibilidade com versões anteriores do plug-in!*
* Rearquitetura da base de código interna para melhorar o desempenho e a estabilidade do plug-in
* Interface de usuário remodelada para aprimorar a experiência geral do usuário
* Interface adicionada para fornecer a capacidade de modificar a divisão em blocos padrão
* Adição de suporte para atualização de texturas na exibição de renderização de ciclos
* Adicionada manipulação de erros no console para notificar se uma substância falhou ao carregar
* Menu flutuante atualizado com ações rápidas

**Seção De Preferências: Adicionada/Atualizada:**

* Parâmetro Exportar formato de imagem; quando imagens geradas no Blender são usadas como entradas de imagem para um material Substance, esse formato é usado para salvar essa imagem na pasta Temporal.
* Caminho da biblioteca Sbsar; especifica a pasta que é aberta por padrão quando o botão Carregar é usado para procurar um arquivo substance.
* Um caminho de exportação de textura padrão (pasta Temporal) que emula o caminho usado pelo Substance 3d Painter para manipular as exportações de arquivos não salvos
* Textura o caminho relativo como acima, com a opção de usar chaves como $matName para criar subpastas
* Caminho relativo dos arquivos sbsar para criar uma subpasta que empacota os arquivos sbsar usados em seu arquivo de mesclagem quando você salva seu projeto
* Capacidade de definir dinamicamente diferentes redes de sombreador nas preferências - Na rede de sombreador, capacidade de definir diferentes variáveis por sombreador dependendo das necessidades de sombreador
* Na seção Saídas da rede de sombreador, você pode definir se uma saída está ativada por padrão
* Capacidade de definir o espaço de cores (ele oferecerá suporte a fluxos de trabalho de dados de aces, exr linear e mesclador, não apenas a srgb)
* A seleção padrão do formato de imagem e da profundidade de bits
* Uma saída genérica para configurar os valores para usos de saída não definidos no sombreador, por exemplo, se você tiver outra saída que não seja usada por padrão pelo sombreador, por exemplo, como uma máscara.
* Um filtro para alterar o tipo de saídas (1 Somente saídas ativadas, 2 Todas as saídas que estão no sombreador e no Substance, 3 Todas as saídas disponíveis no Substance)
* Suporte a atalhos personalizados (editado)

**Seção Do Painel Do Substance 3D: Adicionada/Atualizada:**

* Capacidade de ajustar e bloquear o valor do parâmetro de divisão em blocos gráficos e resolução
* Interface do usuário predefinida atualizada - A lista suspensa Tipo de sombreador para alterar o tipo de gráfico que os usuários desejam ter
* O parâmetro de entrada de imagem foi alterado para a entrada de imagem padrão usada no Blender. Agora, você pode usar imagens do mesclador e não apenas arquivos
* Capacidade de trabalhar em várias instâncias do Blender a qualquer momento
* Suporte para realce automático dos materiais no painel do Substance 3D quando o material é selecionado no visor
