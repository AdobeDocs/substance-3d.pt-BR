---
helpx_url: "https://helpx.adobe.com/br/substance-3d-bake/features/gpu-raytracing.html"
breadcrumb-title: ''
description: Permita que o Rastreamento de raios do GPU acelerado por hardware acelere os cálculos de cozimento em 25x ou mais para workflows mais rápidos.
helpx_creative_field: ""
helpx_description: bakers > Features > GPU Raytracing
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Rastreamento de raios do GPU
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 18%

---


# Rastreamento de raios do GPU

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

Alguns padeiros oferecem suporte à aceleração por hardware do rastreamento de raios na GPU, o que geralmente aumenta a velocidade de computação em um fator de 25 ou mais.

## Requisitos de hardware

O traçado de raio será habilitado automaticamente se o sistema seguir estes requisitos:

* Uma GPU compatível está instalada\* (RTX series, Titan V ou GeForce 10xx)
* Os drivers de GPU estão atualizados
* Windows 10 &#39;Fall Creator&#39; / atualização de outubro (ver 1809) ou superior está instalado\*\*

</td>
<td style="border: 0;" valign="top">

![comparação Rastreamento de raios do GPU ativado/desativado](../../assets/rtx-ao-demo.gif "comparação Rastreamento de raios do GPU ativado/desativado"){zoomable="yes"}

</td>
</tr>
</table>

\*: as GPUs NVIDIA compatíveis incluem todas as GPUs que usam a arquitetura Pascal ou mais recentes. Ou seja, as séries GTX 10, Titan V, RTX 20 ou mais recentes.

\*\*: para verificar sua versão do Windows, clique no menu Iniciar, digite &#39;winver&#39; e pressione Enter.\
Você pode obter a atualização por meio da [página dedicada](https://support.microsoft.com/en-us/help/4028685/windows-10-get-the-update) no site de suporte da Microsoft.

>[!TIP]
>
> Caso você tenha problemas, o Rastreamento de raios do GPU pode ser desativado nas preferências do aplicativo.

## Padeiros com suporte

As tabelas abaixo listam o suporte de Rastreamento de raios do GPU para cada padeiro, de acordo com a versão dos padeiros da Substance 3D:

+++Versão 3 e superior

| Baking | Suporta Rastreamento de raios do GPU |
| --- | --- |
| Oclusão Ambiente | <div><img alt="(assinalar)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Dobra normal | <div><img alt="(assinalar)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Cor | <div><img alt="(assinalar)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Curvatura | <div><img alt="(assinalar)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Altura | <div><img alt="(assinalar)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Normal | <div><img alt="(assinalar)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Espaço mundial normal | <div><img alt="(erro)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |



| Baking | Suporta Rastreamento de raios do GPU |
| --- | --- |
| Máscara de opacidade | <div><img alt="(assinalar)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Posição | <div><img alt="(assinalar)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Posição baixa | <div><img alt="(erro)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |
| Espessura | <div><img alt="(assinalar)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Textura transferida | <div><img alt="(assinalar)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> |
| Mundo em tangente | <div><img alt="(erro)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |


+++

+++Versão 2

| Baking | Suporta Rastreamento de raios do GPU |
| --- | --- |
| Oclusão Ambiente | <div><img alt="(erro)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |
| Oclusão de ambiente da malha | <div><img alt="(assinalar)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> \* |
| Normais dobrados da malha | <div><img alt="(assinalar)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> \* |
| Cor da malha | <div><img alt="(erro)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> \* |
| Converter UV para SVG | <div><img alt="(erro)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |
| Curvatura da malha | <div><img alt="(assinalar)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> \* |
| Altura da malha | <div><img alt="(erro)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> \* |
| Normal da malha | <div><img alt="(erro)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> \* |



| Baking | Suporta Rastreamento de raios do GPU |
| --- | --- |
| Máscara de opacidade da malha | <div><img alt="(erro)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> \* |
| Posição da malha | <div><img alt="(erro)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> \* |
| Posição | <div><img alt="(erro)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |
| Espessura da malha | <div><img alt="(assinalar)&quot; data-preserve-html=&quot;true" src="../../assets/check.svg"/></div> \* |
| Textura transferida partir da Malha | <div><img alt="(erro)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> \* |
| Direção do espaço mundial | <div><img alt="(erro)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |
| Normais do espaço mundial | <div><img alt="(erro)&quot; data-preserve-html=&quot;true" src="../../assets/error.svg"/></div> |


\*: Suporta Rastreamento de raios da CPU, que é significativamente mais lento que o Rastreamento de raios do GPU.

+++
