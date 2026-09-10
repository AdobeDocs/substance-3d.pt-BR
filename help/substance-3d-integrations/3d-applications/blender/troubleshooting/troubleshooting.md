---
helpx_url: "https://helpx.adobe.com/substance-3d-integrations/3d-applications/blender/troubleshooting.html"
breadcrumb-title: ''
description: Diagnostique e resolva problemas comuns com o complemento do Substance 3D no Blender usando o console do sistema.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > 3D Applications > Blender > Troubleshooting
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Solução de problemas
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---


# Solução de problemas

O console do sistema pode ser usado para diagnosticar erros encontrados durante o uso do complemento. A janela do console do sistema do Blender é aberta de forma diferente dependendo do seu sistema operacional. Para obter instruções detalhadas, siga as etapas na [página de documentação](https://docs.blender.org/manual/en/2.79/advanced/command_line/introduction.html#console-window-status-and-error-messages) do console do sistema do Blender. A saída do console pode ser útil ao encontrar problemas inesperados, como texturas que não estão sendo carregadas ou materiais travados no processamento.

Para relatar um erro, ingresse no canal #substance-blender-beta no [servidor do Substance Discord](https://discord.com/invite/substance3d) ou visite as [comunidades de Adobe](https://community.adobe.com/t5/substance-3d-plugins/ct-p/ct-substance-3d-plugins?page=1&sort=latest_replies&lang=all&tabid=all&topics=label-blender). Informações relevantes do registro do console e quaisquer etapas de reprodução para o problema podem ser incluídas nos relatórios.

## Problemas comuns e soluções

* *Erros de console relacionados ao WMIC.*
  * *Ocasionalmente, as instalações do Windows não incluirão o WMIC, que é necessário neste caso. Veja como corrigir isso manualmente:*
    * Acesse Configurações - Sistema - Recursos opcionais
    * Selecione “Exibir recursos” e, em seguida, selecione “Adicionar recurso de opção”
    * Isso trará uma nova janela, percorrerá a lista para baixo para localizar WMIC, marque a caixa de seleção e pressione próximo, na próxima janela pressione Adicionar.
    * Você deve agora ser levado a uma nova janela que mostra o progresso da instalação WMIC sob ações recentes.
    * *Observe que isso pode levar alguns minutos para ser baixado. Depois disso, reinicie o computador e o Blender e o complemento. Quando você clica no carregamento no Painel do Substance 3D, a janela do navegador de arquivos agora deve ser exibida.*
  * Se isso não resolver o problema, talvez você também precise definir WMIC nas variáveis PATH. Consulte a documentação para obter a sua versão específica do Windows.
* *Nem todas as configurações aparecem no Painel do Substance 3D após atualizar o complemento e carregar um material.*
  * Isso pode acontecer ao remover uma versão mais antiga do complemento e instalar uma versão mais nova na mesma sessão, pois os arquivos mais antigos ainda podem estar armazenados em cache no sistema.\
    Reiniciar o Blender deve permitir que as alterações tenham efeito.
* *Problemas ao instalar o complemento./ Os materiais estão travados no processamento entre as sessões. / Os materiais não geram texturas entre as sessões. / Erros ao carregar arquivos .sbsar.*
  * Isso pode ser um problema com a instalação das ferramentas de integração e, geralmente, é corrigido removendo manualmente as ferramentas. Visite a página [Desinstalando o Complemento](../../../3d-applications/blender/uninstalling-the-add-on/uninstalling-the-add-on.md) para obter instruções de remoção manual.
* *Os materiais não são atualizados na exibição de renderização de Ciclos*.
  * Por padrão, o complemento não atualiza as texturas na exibição de renderização Ciclos. No entanto, elas podem ser atualizadas à força ativando-se <b>texturas de atualização automática de ciclos</b>nas preferências do complemento.
* Os parâmetros parecem ser revertidos após salvar na exibição de renderização Ciclos.
  * Esse é um problema de cache conhecido no lado do Blender que é apenas visual. Ao salvar, nenhuma mensagem está sendo enviada ao mecanismo remoto para atualizar os arquivos de textura gerados. As texturas parecerão normais depois de sair da exibição de renderização Ciclos e alternar de volta para ela.
* *Os materiais não estão mais sendo atualizados após desfazer/alterar os parâmetros.*
  * Os materiais podem falhar ao serem atualizados após desfazer as ações. Embora os parâmetros revertam para o estado anterior, as texturas não são desfeitas para corresponder. Para fazer a atualização da textura novamente, use o botão atualizar para retornar os parâmetros para o padrão e recarregar as texturas.
* *As cores definidas no Substance Designer aparecem de forma ligeiramente diferente no seletor de cores do Blender, e os valores de cor não são os mesmos.*
  * O Blender aplica uma correção de gama às cores somente no seletor de cores do Blender. Embora isso cause uma discrepância no seletor de cores, as cores exibidas no textura são precisas aos valores definidos nos aplicativos Substance.
* Erro de console “wmic is not recognition” do *ao carregar um material no Windows.*
  * Esse problema ocorre quando C:\Windows\System32\wbem\ não está incluído nas variáveis de sistema PATH. Consulte a documentação para obter a sua versão específica do Windows.
* *erro “Tipo de CPU inválido é executável” no Mac.*
  * Esse problema ocorre quando o Rosetta não está ativado em computadores Mac ARM. Consulte a [página Rosetta do Apple](https://support.apple.com/en-us/102527) para obter mais informações. Além disso, consulte este [guia de instalação](https://medium.com/@jithmisha/fix-for-macbook-air-m1-m2-bad-cpu-type-in-executable-error-3719a0a1cb6) para obter mais instruções.
* *As modificações no gráfico de sombreador são desfeitas ao usar o botão Atualizar ou ao atualizar parâmetros.*
  * O complemento atualizou as conexões no gráfico após alterações ou atualizações. Para contornar esse problema, duplique o material de mesclagem criado a partir do .sbsar e dê a ele um novo nome de sua escolha. Adicione seus nós somente à duplicata. As texturas serão atualizadas no grupo de nós enquanto os nós adicionados pelo usuário são mantidos. Ao atualizar, copie esses nós e cole-os novamente em um novo gráfico após a atualização.
