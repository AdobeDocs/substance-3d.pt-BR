---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/3d-applications/blender/preferences.html"
breadcrumb-title: ''
description: Configure as preferências do complemento do Substance 3D no Blender para personalizar o comportamento e as configurações do plug-in.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > Preferences
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Preferências
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 0%

---


# Preferências

As preferências do complemento podem ser encontradas na janela de preferências do Blender. Navegue até Editar > Preferências > Complementos e pesquise por Nó: Complemento Adobe Substance 3D para Blender.

<table>
<tr style="border: 0;">
<td style="border: 0;" valign="top">

![Primeira metade do menu de preferências do complemento.](../../../assets/blender-prefs-1.png)

</td>
<td style="border: 0;" valign="top">

![Segunda metade do menu de preferências do complemento.](../../../assets/blender-prefs-2-b.png)

</td>
</tr>
</table>

<b>Desinstalar</b> - Exclui o complemento do sistema e o remove da lista de complementos no Blender.

<b>Relatar um erro</b> - abre o Substance 3D para o Blender Discord.

<b>Aceitar pasta de ferramentas</b> - Abre o navegador de arquivos do Blender para escolher o caminho de instalação das Ferramentas de Integração do Substance.

<b>Abrir Ferramentas </b>- Abra o navegador de arquivos do sistema no local da pasta Ferramentas de Integração.

<b>Redefinir Caminho</b> - Redefine o caminho da pasta Ferramentas de Integração para o local padrão.

<b>Ferramentas de Desinstalação</b> - Remove a versão instalada das Ferramentas de Integração do Substance 3D.

<b>Atualizar Ferramentas</b> - Abre o navegador de arquivos para selecionar o arquivo zip de ferramentas e atualizar as ferramentas.

<b>Documentação</b> - abre a página de documentação de Ecossistema e Plug-ins no navegador.

<b>Fóruns</b> - Abre os Fóruns da comunidade do Adobe no navegador.

<b>Discord Server</b> - Abre o servidor Ecosystem and Plugins Discord no navegador.

<b>Divisão em blocos gráficos</b> - Ajuste a divisão em blocos gráficos X, Y e Z do material. O bloqueio pode ser usado para desvincular os valores e ajustá-los individualmente.

<b>Resolução</b> - A resolução padrão para texturas geradas. O bloqueio pode ser usado para desvincular a fim de definir suas resoluções de maneira independente.

<b>Aplicar Tipo </b>- Define o comportamento do botão Aplicar: <b>Inserir </b>substituirá o material atual pelo material de Substance selecionado e <b>Acrescentar</b> adicionará o material ao objeto em um novo slot de material.

<b>Formato de exportação de imagem</b> - Quando imagens geradas no Blender são usadas como entradas de imagem para um material Substance, esse formato é usado para salvar essa imagem na pasta temporal.

<b>Grupos de entrada recolhidos por padrão</b> - Alterna o clima porque os grupos de entrada do material de Substance são expandidos ou recolhidos por padrão.

<b>Somente atualizar texturas por padrão</b> - alterna os parâmetros de Substance de atualização de clima afeta apenas as texturas de saída na rede do Sombreamento do Blender. Desabilitar isso redefinirá as conexões de nó depois de ajustar os parâmetros. A ativação é recomendada ao adicionar nós adicionais a um material, caso contrário, eles serão desconectados após o ajuste dos parâmetros.

<b>Mecanismo Remoto do Substance </b>- Define o hardware usado pelo Mecanismo Remoto do Substance.

<b>Aplicar automaticamente o material</b> - Quando um material de Substance é criado, anexe automaticamente o material ao(s) objeto(s) selecionado(s) em um novo slot de material.

<b>Realçar automaticamente o material dos objetos selecionados</b> - Altere o material realçado no painel do Substance 3D se um objeto com esse material for selecionado.

<b>Atualização automática de texturas de ciclos</b> - Força a atualização da textura na Janela de Visualização 3D ao usar a exibição de renderização de Ciclos.

<b>Confirmação de exclusão de predefinição</b> - Remove a janela de confirmação que aparece ao excluir predefinições de material.

<b>Criar material com usuário falso habilitado</b> - Define o clima em que o material é criado com “usuário falso” habilitado ou desabilitado. Os dados do mesclador marcados como usuário falso não são removidos após o fechamento, mesmo quando os dados não são usados.

<b>Iniciar automaticamente o Mecanismo Remoto do Substance </b>- Ativa/desativa a inicialização do Mecanismo Remoto do Substance quando o Blender é iniciado. Se desabilitado, o mecanismo remoto só será iniciado quando um botão de carregamento do usuário ou usar o atalho de carregamento.

>[!NOTE]
>
> OBSERVAÇÃO: se estiver usando o Substance Connector, o SRE deverá estar ativo para que o aplicativo de envio detecte o Blender como um ponto de extremidade.

<b>Caminho da biblioteca SBSAR</b> - A pasta que é aberta por padrão quando o botão Carregar pesquisa um arquivo substance.

<b>Pasta Temporária </b>- Esta pasta será o local padrão onde as texturas são armazenadas antes de um arquivo ser salvo pela primeira vez.

<b>Copiar arquivos .sbsar ao salvar em</b> - Quando habilitado, os arquivos .sbsar são copiados para o caminho relativo especificado quando o arquivo é salvo. Isso pode facilitar o compartilhamento de projetos entre dispositivos.

<b>Ao salvar, copie as texturas para</b> - Quando um arquivo for salvo pela primeira vez, as texturas na pasta temporária serão copiadas para este local. A variável $matname é usada para criar subpastas para cada material.

<b>Predefinição de sombreador</b> - Define a predefinição de sombreador padrão usada ao criar materiais do Misturador a partir de arquivos de substâncias. Pode ser definido como padrão para mapeamento baseado em UV ou projeção para mapeamento baseado em caixa, esfera e cilindro.

<b>Nível Médio do Deslocamento</b> - O valor padrão é a base para o deslocamento no Nó do Deslocamento. Valores maiores que o padrão empurrarão superfícies para fora e valores menores que o padrão puxarão superfícies para dentro.

<b>Escala de Deslocamento</b>- O valor de escala padrão no nó de Deslocamento.

<b>Intensidade da Emissão</b> - O valor padrão para a Intensidade da Emissão no nó Principled BSDF.

<b>Mesclagem de projeção</b> - Define a quantidade de mesclagem entre ângulos para os sombreadores do método de projeção.

<b>Mix de AO</b> - Quando a Oclusão ambiente está habilitada como saída, esse valor determina o valor de fator padrão do nó MixRGB usado para combinar as texturas de Cor base e Oclusão ambiente.

<b>Saídas</b> - As saídas individuais de materiais podem ser habilitadas ou desabilitadas. O espaço de cores padrão, o formato de arquivo e a profundidade de cores de saídas individuais também podem ser ajustados.

<b>Atalhos </b>- Personalize as teclas de atalho usadas para abrir um menu flutuante, carregar um material de Substance e aplicar o material atual. As atualizações de atalho exigem uma reinicialização para entrar em vigor.
