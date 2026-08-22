---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/game-engines/roblox.html"
breadcrumb-title: ''
description: Use materiais de Substance no Roblox Studio com o fluxo de trabalho Aspereza metálica PBR para experiências 3D imersivas.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Roblox
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Roblox
user-guide-description: ''
user-guide-title: ''
source-git-commit: 4a060ee1aaa1731c04e70d5512e3271cd63d0381
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---


# Roblox

O [Roblox](https://www.roblox.com/) é uma plataforma para experiências imersivas e multiplayer em 3D. O Roblox Studio, a ferramenta de design Roblox, suporta o fluxo de trabalho Aspereza metálica PBR.

<table>
<tr style="border: 0;">
<td width="58.30%" style="border: 0;" valign="top">

## Modelo do Substance 3D Designer

Para criar texturas para o Roblox, você pode usar o arquivo do Substance 3D abaixo como um modelo de [gráficos de composição de Substance](https://experienceleague.adobe.com/pt-br/docs/substance-3d-designer/using/substance-graphs/substance-compositing-graphs) no [Substance 3D Designer](https://experienceleague.adobe.com/en/docs/substance-3d-designer/home).

[![Imagem do ícone de formato de arquivo sbs vinculada ao modelo roblox.](../../assets/sbs.png){width="64px"}](https://helpx.adobe.com/content/dam/roblox.sbs)

Este modelo de gráfico permite a pré-configuração dos nomes e tipos finais dos arquivos de textura. Este modelo pode ser instalado e reutilizado para criar novos materiais que sempre seguem as diretrizes de materiais do Roblox.

</td>
<td width="41.60%" style="border: 0;" valign="top">

![](https://helpx-prod.scene7.com/is/image/HelpxProd/roblox-template?$png$&jpegSize=100&wid=401){width="200px"}

</td>
</tr>
</table>

## Fluxo de trabalho Designer para Roblox

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

### Instalar modelo

Primeiro, *instale* o modelo Roblox.

* Baixe o arquivo de modelo vinculado acima.
* Acesse o diretório de documentos do usuário do Designer:
* (Creative Cloud Desktop) `/Documents/Adobe/Adobe Substance 3D Designer`\
  (Vapor) `/Documents/Allegorithmic/Substance Designer/`
* Crie uma pasta de modelos.
* Coloque o arquivo nessa pasta.

</td>
<td style="border: 0;" valign="top">

![](../../assets/roblox-01-place-template.gif){width="512px"}

</td>
</tr>
</table>

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

### Detectar modelo

Depois, peça ao Designer *assistir* à pasta de modelos para procurar modelos de gráfico.

* No Designer, vá para **Editar > Preferências...**
* Na janela [Preferências](https://experienceleague.adobe.com/pt-br/docs/substance-3d-designer/using/workspace/preferences/preferences-window), vá para **Projetos > Projeto de usuário > Geral**
* Na lista **Diretórios de Modelos**, clique no botão **+**
* Vá para o diretório `templates` e clique em **Selecionar pasta**
* Clique no botão **OK**
* Vá para **Arquivo > Novo > gráfico de Substance...**
* Verifique se o modelo `Roblox` está listado na parte inferior da lista de modelos na janela [Novo Substance](https://helpx.adobe.com/br/substance-3d/unlisted/documentation/sddoc/create-a-graph-102400068.html)

</td>
<td style="border: 0;" valign="top">

![](../../assets/roblox-02-detect-template.gif){width="512px"}

</td>
</tr>
</table>

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

### Exportar texturas

Crie um gráfico usando o modelo Roblox e exporte bitmaps desse gráfico quando terminar de trabalhar em um material.

* Na janela [Novo gráfico de Substance](https://helpx.adobe.com/br/substance-3d/unlisted/documentation/sddoc/create-a-graph-102400068.html), selecione o modelo `Roblox`
* Defina qualquer identificador e outros parâmetros para o gráfico e clique em **OK**
* Trabalhe no seu material na [Exibição de gráfico](https://experienceleague.adobe.com/pt-br/docs/substance-3d-designer/using/workspace/graph-view/the-graph-view) - veja [aqui](https://experienceleague.adobe.com/pt-br/docs/substance-3d-designer/using/getting-started/workflow-overview) para começar a usar o fluxo de trabalho
* Quando terminar, vá para **Ferramentas > Exportar bitmaps...** na Exibição de gráfico *barra de ferramentas*
* Na janela [Exportar bitmaps](https://experienceleague.adobe.com/pt-br/docs/substance-3d-designer/using/substance-graphs/exporting-bitmaps), defina um caminho válido de **Destino**, verifique se *todas* as saídas estão *marcadas* e clique em **Exportar**
* Verifique se as texturas são exportadas corretamente para o caminho de **Destino**

</td>
<td style="border: 0;" valign="top">

![](../../assets/roblox-03-export-textures.gif){width="512px"}

</td>
</tr>
</table>

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

### Criar material no Roblox

No Roblox, crie uma Variante de material e atribua as texturas exportadas do Designer.

* Selecione a guia **Modelo** e clique em **Gerenciador de materiais**
* Selecione um *modelo de material* e clique no botão **Criar Variante**
* Na janela **Criar variante**, defina um nome para o material
* Para *cada canal de material*, clique no botão **Importar** e selecione a textura correspondente exportada do Designer
* Clique em **Salvar**

</td>
<td style="border: 0;" valign="top">

![](../../assets/roblox-04-roblox-create-material.gif){width="512px"}

</td>
</tr>
</table>

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

### Aplicar material

Use sua nova variante de material na cena do Roblox

* *Selecione* qualquer parte ou malha em sua cena do Roblox
* No **Gerenciador de Materiais**, selecione sua *variante de material* e clique no botão **Aplicar às Partes Selecionadas**

>[!NOTE]
>
> Se a cor das texturas parecer diferente no Roblox, verifique o atributo **Cor** na categoria **Aparência** nas propriedades do objeto ao qual a Variante de material está aplicada e certifique-se de que esteja definida como *branco puro*, ou seja, RGB (255, 255, 255), rotulado como *Branco institucional* no Roblox.

</td>
<td style="border: 0;" valign="top">

![](../../assets/roblox-05-roblox-apply-material.gif){width="512px"}

</td>
</tr>
</table>

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

### Ajustar divisão em blocos gráficos

A quantidade de repetição do material em uma superfície - ou seja, azulejos - pode ser ajustada a qualquer momento.

* No **Gerenciador de Materiais**, selecione sua *variante de material* e clique no botão **Editar**
* Na janela **Editar Variante**, ajuste o valor da propriedade **Pinos por Bloco** em **Adicional** - um valor *inferior* resulta em *mais* repetição

</td>
<td style="border: 0;" valign="top">

![](../../assets/roblox-06-roblox-adjust-tiling.gif){width="512px"}

</td>
</tr>
</table>
