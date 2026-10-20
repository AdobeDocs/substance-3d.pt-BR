---
title: Blender add-on 3.0.0+
description: Uma lista de notas de versão do plug-in Substance 3D para Blender.
source-git-commit: 1488c476be7921c113d2a54f870fee090e6295e9
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%
---

# Complemento 3.0.0+

**Complemento 3.1.0**.*Lançado em: 20 de outubro de 2026*

**Complemento do Blender:**

* &amp;lbrack;Bug&amp;rbrack; O caminho fixo da biblioteca não está funcionando
* &amp;lbrack;Bug&amp;rbrack; Problema de contexto corrigido em multithreading, faz com que o SBSAR não carregue/atualize
* &amp;lbrack;Bug&amp;rbrack; O formato de exportação de Textura fixa é ignorado
* &amp;lbrack;Desempenho&amp;rbrack; Várias melhorias de desempenho

**Ferramentas de Integrações de Substance (Substance Remote Engine):**

* &amp;lbrack;Feature&amp;brack; Atualizado para o Substance Engine 9.6.1
* &amp;lbrack;Desempenho&amp;rbrack; Dependências atualizadas e várias melhorias de desempenho

**Complemento 3.0.1**.*Lançado em: fevereiro de 2026*

**Complemento do Blender:**

* &amp;lbrack;Fixo&amp;rbrack; Os valores mínimos/máximos dos parâmetros não estão funcionando
* &amp;lbrack;Fixo&amp;rbrack; Tamanho físico não funciona com escala de cena personalizada
* &amp;lbrack;Fixo&amp;rbrack; Tamanho físico não funciona com unidades do sistema não métricas
* &amp;lbrack;Fixo&amp;rbrack; Mapas de revestimento não funcionam com o blender 4+
* &amp;lbrack;Fixed&amp;rbrack; Mapa de cores de revestimento ausente no sombreador
* &amp;lbrack;Fixed&amp;rbrack; Rótulo incorreto na definição do AddOn
* &amp;lbrack;Fixo&amp;rbrack; Substance faz com que o SRE trave aleatoriamente (com valores de color float4)
* &amp;lbrack;Fixo&amp;rbrack; As entradas de imagem não são exibidas na lista de parâmetros
* &amp;lbrack;Fixo&amp;lbrack; As entradas da imagem não funcionam após fechar e reabrir o liquidificador

**Ferramentas de Integrações de Substance (Substance Remote Engine):**

* Atualize para a versão 3.0.1
* Remoção da ABI C++11 para a nova compilação do Linux
