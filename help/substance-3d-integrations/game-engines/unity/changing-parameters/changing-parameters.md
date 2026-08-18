---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/game-engines/unity/changing-parameters.html"
breadcrumb-title: ''
description: Modifique os parâmetros de material de Substance no Unity para personalizar a aparência e as propriedades do material no tempo de execução.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unity > Changing parameters
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Alterando parâmetros
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 0%

---


# Alterando parâmetros

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

Os parâmetros para o material de Substance estão acessíveis no SGO (Gráfico do Substance Object).

1. Na janela Projeto, selecione o logotipo do arquivo sbsar do gráfico que deseja personalizar. A sbsar tem o logotipo verde “SBSAR”.

   ![](../../../assets/screen-shot-2022-03-29-at-2-27-56-pm.png)

## Propriedades de procedimento

1. **Gerar todas as saídas**: gera todas as saídas do arquivo Substance sbsar. Por padrão, apenas as saídas usadas pelos sombreadores padrão são criadas.
1. **Gerar Mipmaps**: irá gerar texturas mip para cada saída de Substance.
1. **Distribuição aleatória**: este botão alterará a distribuição aleatória que o gráfico de Substance usa para gerar as texturas. Alterar esse valor criará um novo resultado para a textura calculada com base no valor de semente.
1. Os parâmetros expostos no arquivo Substance estão disponíveis no Unity. O controle Editor é baseado no tipo de parâmetro criado para o Substance.
1. **Tratamento de predefinições:** você pode exportar ou importar arquivos de predefinições de Substance (sbsars). A exportação de uma predefinição criará um arquivo de predefinição com base nas configurações de parâmetro do Substance. É possível exportar arquivos de predefinição de Substance Designer e Substance Player que podem ser importados usando o botão Importar predefinição. Isso é útil para compartilhar predefinições de Substance entre aplicativos e equipes.

</td>
<td style="border: 0;" valign="top">

![](../../../assets/changing-parameters.png)

</td>
</tr>
</table>
