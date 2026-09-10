---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/blender/release-notes/blender-add-on-2-0-0.html"
breadcrumb-title: ''
description: Consulte as notas de versão do complemento do Blender versão 2.0.0 para saber mais sobre novos recursos, aprimoramentos e correções de erros.
helpx_creative_field: ""
helpx_description: Substance 3D Integrations
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Complemento 2.0.0
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---


# Complemento 2.0.0

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
