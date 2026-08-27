---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/blender/release-notes/add-on-0-9-3/add-on-2-0-0-plus.html"
breadcrumb-title: ''
description: Revise as notas de versão do complemento do Blender versão 2.0.0 e posterior para saber mais sobre novos recursos e melhorias.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > Release Notes > Add-on 2.0.0
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Complemento 2.0.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 0%

---


# Complemento 2.0.0+

## Complemento 2.2

<b>Adicionado:</b>

* Suporte para renderizador de octano
* Suporte inicial ao Redshift
* Suporte inicial para o Renderman

<b>Atualizado:</b>

* Atualizado para a versão mais recente do conector
* Funcionalidade adicionada para receber predefinições usando o conector
* Aprimoramento da funcionalidade de predefinição de importação: agora, todas as instâncias de um SBSAR que incluem o material adicionarão a predefinição
* Funcionalidade padronizada do conector

<b>Corrigido:</b>

* Erro de persistência em que a imagem de entrada não funcionava após salvar o arquivo de mesclagem
* Problema com a rede do sombreador que não funciona ao atualizar a predefinição do sombreador
* URL incorreta no botão de plug-in de download
* Ladrilho invertido em octano
* Valores de entrada não funcionais com renderizadores de terceiros
* Problema em que o parâmetro de valor de entrada float não foi criado
* Os espaços de cores do Renderman não estão funcionando corretamente
* As predefinições de sombreador não estão sendo filtradas pelo renderizador disponível

## Complemento 2.1.1

Esta atualização inclui compatibilidade com o Blender 4.0+ e vários recursos novos nas Preferências de complemento. Também adicionamos suporte ao Substance Connector para a transferência de dados sem problemas entre o Substance 3D Sampler e o Blender (Enviar para) e resolvemos alguns erros. Localize as notas de versão detalhadas abaixo.

<b>Adicionado/Atualizado:</b>

* Adição da funcionalidade do conector do Substance (compatível com arquivos SBSAR e arquivos USD).
* Suporte para o Blender 4.0+.
* Suporte para SRE versão 2.1.0.
* Em Preferências de Complemento:
  * Capacidade de escolher o caminho de instalação das Ferramentas de Integração do Substance.
  * Botão para redefinir as Ferramentas de Integração para o caminho padrão.
  * Botão para abrir a pasta Ferramentas de integração.
  * Adicionado Aplicar tipo para atribuir material (Inserir: defina-o como material principal, Anexar: adicione-o na parte inferior da lista).
  * Adicionada caixa de seleção para selecionar o comportamento padrão dos grupos de Entrada (recolhida/expandida).
  * Adicionada caixa de seleção para selecionar o comportamento padrão da propriedade atualizar somente texturas.
  * Inicie automaticamente o Substance Remote Engine ao abrir o Blender (importante para ser ativado se estiver usando o conector).
* Complemento:
  * Adicionada somente texturas de atualização (permite alterar os parâmetros sem refazer o gráfico de nó).
  * Adicionado, expandir todos os grupos e recolher todos os botões de grupos.
  * Grupo de imagens de entrada adicionado para agrupar todas as imagens de entrada, se necessário, em um SBSAR.
  * As Entradas de parâmetro agora são exibidas na mesma ordem que o Designer.
  * Adicionada a visualização em miniatura de cada material de Substance.

<b>Corrigido:</b>

* O bug do grupo de entrada Geral vazio foi corrigido.

<b>Problemas Conhecidos:</b>

* A funcionalidade de selecionar automaticamente o SBSAR ao selecionar um objeto não está funcionando no momento, portanto, está desativada.

## Complemento 2.0.0

O Complemento Substance 3D 2.0 marca uma atualização transformadora para usuários do Blender, apresentando uma arquitetura de plug-ins completamente refatorada. Esse novo design se concentra na integração perfeita, no desempenho aprimorado e em uma base flexível para futuras expansões. Representa não apenas uma atualização, mas uma reimaginação de como os materiais de Substance são tratados no Blender, atendendo às necessidades em evolução dos profissionais 3D.

<b>Destaques da versão 2.0:</b>

* Arquitetura refatorada: estrutura aprimorada de plug-ins para desempenho e integração aprimorados
* Suporte a futura expansão - a atualização estabelece as bases para a adição fácil de novos recursos no futuro
* Compatibilidade mais ampla - totalmente compatível com as versões 3.0 e posteriores do Blender, incluindo suporte para usuários do Mac

<b>Adicionado/Atualizado:</b>

* [SRE] Suporte à seleção de Substance Engine (GPU é o padrão)
* [SRE] Novos formatos de imagem para exportar as texturas
* [SRE] Profundidade de bits seleção para cada tipo de mapa
* [BLD] Suporte a saídas de valor
* [BLD] Suporte à entrada de cadeia de caracteres
* [SRE] Opção adicionada para selecionar a pasta temporária padrão para o destino de exportação da imagem

<b>Corrigido:</b>

* [SRE] Melhoria geral do desempenho
* [BLD] Correção de problemas de comunicação entre as Ferramentas de integração e o Blender
* [BLD] Falha ao instalar/iniciar as Ferramentas de Integração
* [BLD] As ferramentas de integração não terminam ao fechar o Blender
* [BLD] Material não atualizado ao alterar o tipo de arquivo de um mapa
* [SRE] Todos os mapas dos materiais são exportados o tempo todo
* [SRE] As ferramentas de integração exportam mapas normais com degraus
* [SRE] A carga do Substance nunca termina
* [SRE] As unidades do Tamanho físico não são ajustadas para a cena
* [BLD] As predefinições geradas no Blender não funcionam com outras integrações
* [BLD] O material não é atualizado em ciclos
* [BLD] Os limites flexível e rígido das entradas são ignorados
* [BLD] A intensidade da cor não é atualizada corretamente ao ajustar um parâmetro
* [SRE] Falha na desinstalação das Ferramentas de Integração
* [SRE] Corrigimos o problema no qual a duplicação de materiais várias vezes causava erro.
* [SRE] O espaço de cores dos nós de imagem agora corresponde corretamente às preferências do usuário.

<b>Problemas conhecidos:</b>

* Ao usar o Blender v4.0+, os soquetes não estão em ordem após serem ativados e desativados várias vezes
* Cltr+Z para desfazer alterações pode causar erros
* Carregar um arquivo vazio ou uma pasta em vez de um arquivo .sbsar pode interromper o plug-in
* Suporte ao modo Blender sem periféricos
