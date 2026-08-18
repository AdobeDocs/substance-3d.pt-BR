---
helpx_url: "https://helpx.adobe.com/br/substance-3d-integrations/game-engines/unreal-engine/unreal-engine-4/working-with-displacement-ue4.html"
breadcrumb-title: ''
description: Ative o mosaico e use mapas de deslocamento de materiais de Substance em Unreal Engine 4 para obter detalhes de superfície.
helpx_creative_field: ""
helpx_description: Ecosystems and Plugins > Game Engines > Unreal Engine > Unreal Engine 4 > Working with Displacement - UE4
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Trabalhando com o Deslocamento - UE4
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---


# Trabalhando com o Deslocamento - UE4

Para trabalhar com o deslocamento, você precisará ativar o mosaico no material.

![](../../../../assets/tess.png){width="600px"}

Para usar a saída do height, você precisa clicar duas vezes na Saída na Instância do Substance Fatory para criar o height. O height não é ativado por padrão. Em seguida, você pode arrastar a saída dessa height para o material.

![](../../../../assets/height-1.png){width="800px"}

Depois de adicionar a saída do height ao material, você precisará criar alguns nós para orientar o World Deslocamento e o Tessellation Modifier.

1. Crie 2 parâmetros escalares. Um será Distância e o outro será o multiplicador do mosaico.
1. Multiplique o canal Vermelho do Height para o parâmetro Distância
1. Adicione um nó VertexNormalWS e multiplique-o com a saída da multiplicação na etapa 2.
1. Insira a multiplicação de VertexNormal para o Deslocamento de mundo no Material.
1. Use o parâmetro de multiplicador de mosaico e insira-o no Multiplicador de mosaico do material.

![](../../../../assets/setup-3.png){width="800px"}

>[!NOTE]
>
> As outras saídas de textura foram omitidas nesta imagem para simplificar o gráfico. Aqui, apenas os nós Deslocamento e Multiplicador são mostrados para fins de esclarecimento.
