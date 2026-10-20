---
title: Blender add-on 3.0.0+
description: Uma lista de notas de versão do plug-in Substance 3D para Blender.
source-git-commit: aa5acd016cd1a55ab230d36352c4d3aa5514012a
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%
---

# Complemento 3.0.0+

**Complemento 3.1.0**.*Lançado em: 12 de outubro de 2026*

**Complemento do Blender:**

* &lbrack;Bug&rbrack; O caminho fixo da biblioteca não está funcionando
* &lbrack;Bug&rbrack; Problema de contexto corrigido em multithreading, faz com que o SBSAR não carregue/atualize
* &lbrack;Bug&rbrack; O formato de exportação de Textura fixa é ignorado
* &lbrack;Desempenho&rbrack; Várias melhorias de desempenho

**Ferramentas de Integrações de Substance (Substance Remote Engine):**

* &lbrack;Feature&brack; Atualizado para o Substance Engine 9.6.1
* &lbrack;Desempenho&rbrack; Dependências atualizadas e várias melhorias de desempenho

**Complemento 3.0.1**.*Lançado em: fevereiro de 2026*

**Complemento do Blender:**

* &lbrack;Fixo&rbrack; Os valores mínimos/máximos dos parâmetros não estão funcionando
* &lbrack;Fixo&rbrack; Tamanho físico não funciona com escala de cena personalizada
* &lbrack;Fixo&rbrack; Tamanho físico não funciona com unidades do sistema não métricas
* &lbrack;Fixo&rbrack; Mapas de revestimento não funcionam com o blender 4+
* &lbrack;Fixed&rbrack; Mapa de cores de revestimento ausente no sombreador
* &lbrack;Fixed&rbrack; Rótulo incorreto na definição do AddOn
* &lbrack;Fixo&rbrack; Substance faz com que o SRE trave aleatoriamente (com valores de color float4)
* &lbrack;Fixo&rbrack; As entradas de imagem não são exibidas na lista de parâmetros
* &lbrack;Fixo&lbrack; As entradas da imagem não funcionam após fechar e reabrir o liquidificador

**Ferramentas de Integrações de Substance (Substance Remote Engine):**

* Atualize para a versão 3.0.1
* Remoção da ABI C++11 para a nova compilação do Linux