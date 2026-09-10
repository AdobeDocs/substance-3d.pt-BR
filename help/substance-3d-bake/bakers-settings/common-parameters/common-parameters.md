---
helpx_url: "https://helpx.adobe.com/substance-3d-bake/bakers-settings/common-parameters.html"
breadcrumb-title: ''
description: Saiba mais sobre os parâmetros comuns que se aplicam a todos os baker e como configurá-los para geração de textura ideal.
helpx_creative_field: ""
helpx_description: bakers > Bakers Settings > Common Parameters
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Parâmetros comuns
user-guide-description: ''
user-guide-title: ''
source-git-commit: 0197b6f5f4e3ed1f2bc0e5576bd5818d04485ed5
workflow-type: tm+mt
source-wordcount: '1068'
ht-degree: 1%

---


# Parâmetros comuns

Parâmetros comuns se aplicam a todos os baker. Esses parâmetros geralmente definem como os baker se comportarão e trabalharão com malhas de alto-polígono, mas como as texturas finais serão geradas. Alguns desses parâmetros podem ser substituídos por baker específicos.

Embora a maioria desses parâmetros esteja disponível em todos os softwares (incluindo o Substance Automation Toolkit), seu comportamento pode ser ligeiramente diferente; ou alguns deles podem não estar disponíveis dependendo do fluxo de trabalho e da implementação do software.

## Parâmetros gerais

Esses parâmetros afetam a maneira como os baker geram texturas.

| *Nome* | *Descrição* |
| --- | --- |
| **Tamanho**(Tamanho Padrão ou Tamanho de Saída) | Controla a resolução de textura de saída feita bake (em pixels). Valores disponíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>32</strong></li><li data-preserve-html="true"><strong>64</strong></li><li data-preserve-html="true"><strong>128</strong></li><li data-preserve-html="true"><strong>256</strong></li><li data-preserve-html="true"><strong>512</strong></li><li data-preserve-html="true"><strong>1024</strong></li><li data-preserve-html="true"><strong>2048</strong> (padrão)</li><li data-preserve-html="true"><strong>4096</strong></li><li data-preserve-html="true"><strong>8192</strong></li></ul>Resoluções não quadradas também são compatíveis, por exemplo: 2048x1024 (proporção 2:1). No Substance Designer, esse parâmetro pode ser substituído pelo próprio baker. |
| **Formato** | Formato de arquivo das texturas feitas bake.*Não disponível no Substance Painter.* Consulte: [Como exportar os mapas baked](../../common-questions/how-export-the-baked-maps/how-to-export-the-baked-maps.md). |
| **Suavização de borda** | Controla a suavização de serrilhado, que pode melhorar a qualidade das texturas feitas bake e reduzir o serrilhado nos locais em que diferentes geometrias se conectam.Para saber mais sobre aliases, consulte: [Aliases em Seams UV](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md) e [Aliases na Wikipédia](https://en.wikipedia.org/wiki/Aliasing).Valores disponíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Nenhum</strong> (padrão)</li><li data-preserve-html="true"><strong>Subamostragem de 2x2</strong></li><li data-preserve-html="true"><strong>Subamostragem 4x4</strong></li><li data-preserve-html="true"><strong>Subamostragem 8x8</strong></li></ul>  **Observação:** a ativação da suavização de borda pode aumentar significativamente o tempo de fça bake, pois funciona calculando a textura com uma resolução mais alta e reduzindo-a de volta ao tamanho originalmente selecionado. Isso significa que uma textura 2K com uma subamostragem 2x2 calculará uma textura 4K.Às vezes, é preferível aumentar o número de raios no baker em vez de aumentar a subamostragem. Poderia alcançar melhores resultados sem esperar muito. |
| **Conjunto UV** | Controla quais UVs da malha de baixo polígono serão usados para calcular as texturas feitas bake.*Não disponível no Substance Painter.* |
|  |  |
| **Dilatação (px)** | Dilatar/estender os pixels das UVs fora ou de sua borda pela quantidade de pixels fornecida. Esta operação permite evitar emendas nas bordas UV quando essas bordas não estão perfeitamente alinhadas com os pixels da textura ou quando a resolução da textura é reduzida (por exemplo: mipmaps). Este é um pós-processo aplicado após o processo de fça bake. Às vezes, também pode ser chamado de “preenchimento”.Para saber mais sobre dilatação, consulte: [Suavização em emendas UV](../../common-issues/aliasing-on-uv-seams/aliasing-on-uv-seams.md) e [Preenchimento](https://helpx.adobe.com/substance-3d/unlisted/documentation/spdoc/padding-134643719.html). |
| **Aplicar difusão** | Se ativada, a parte externa dos UVs será preenchida com cores de gradiente suavizadas com base nas bordas UV. Esse processo garante que, quando o tamanho da textura for reduzido, ela permanecerá estável e não criará emendas excessivamente visíveis (por exemplo: mipmaps). Este é um pós-processo aplicado após o processo de fça bake. |
| **Média Normalizada** | Se habilitado, calcula o normal médio de um vértice para saber em que direção enviar raios durante o processo de correspondência de malha de fça bake. Se desativado, os raios seguirão os normais de vértice originais da malha. |

## Parâmetros High-Poly

Os parâmetros a seguir controlam o fça bake de malha de alto-poli para baixo-poli (baker de malha).

| *Nome* | *Descrição* |
| --- | --- |
| **Malhas de alta definição** | Uma lista de arquivos (ou recursos de pacote de Substance) que contém malhas de alto polígono. Eles são carregados na memória pelos padeiros quando o processo de cozimento começa a computar informações diferentes e salvar essas informações de malha em texturas. Esta lista será ignorada se “**Usar baixa como alta definição**” estiver habilitado. |
| **Usar Malha Baixa como Alta Definição** ou **Usar Malha Baixa como Malha Alta de Poli** | Se habilitada, a lista de malha de alto-poli fornecida aos padeiros será ignorada e a malha de baixo-poli será assada em si mesma.Esse parâmetro é útil ao trabalhar diretamente com uma malha de alto-polímero. Por exemplo, ao assar uma textura de oclusão ambiente para um carro de alta polivalência com essa configuração ativada, a distância do raio é ignorada e o padeiro produzirá um bolo perfeito (sem erros de raio ou incompatibilidade de geometria). |
|  |  |
| **Definir distância com gaiola** ou **Usar gaiola** | Indica se um arquivo de malha de gaiola deve ser usado no processo de cozimento em vez de usar valores de distância de raio. A gaiola controla a distância e a direção máximas do raio. |
| **Arquivo de caixa** | Caminho do arquivo de malha que contém o compartimento. |
| **Valor Frontal** ou **Distância Frontal Máxima** | Controla o quanto acima da superfície de baixo polígono o raio deve começar a encontrar qualquer geometria de alto polígono ao longo de seu caminho.*Esta configuração não tem efeito quando uma Gaiola é usada.* |
| **Valor traseiro** ou **Distância traseira máxima** | Controla o quanto abaixo da superfície de baixo polígono o raio deve parar para encontrar qualquer geometria de alto polígono ao longo de seu caminho.*Esta configuração não tem efeito quando uma Gaiola é usada.* |
| **Em relação à caixa delimitadora** | Se ativado, a distância de raio e outros cálculos baseados em tamanho são baseados no espaço normalizado da malha de baixo-polímero. Se desativada, o cálculo da distância de raio será baseado em unidades especificadas na malha de baixo polímero quando ela for exportada (metros, centímetros etc.). Às vezes, pode ser útil desativar essa configuração e inserir a distância de raio manualmente quando um objeto tiver medidas precisas. |
|  |  |
| **Corresponder** | Indica como os padeiros devem corresponder à geometria baixa e alta. Ele pode ser usado para filtrar o processo de cozimento sem a necessidade de mover manualmente (explodir) malhas.Valores possíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Sempre</strong> (padrão): a malha de baixo polígono corresponde a cada malha de alto polígono.</li><li data-preserve-html="true"><strong>Por nome da malha</strong>: filtre as malhas por nome para evitar correspondência com geometria indesejada.</li></ul>Para saber mais sobre a geometria correspondente, consulte: [Correspondência por Nome](../../features/matching-by-name/matching-by-name.md). |
| **Sufixos de correspondência** ou **Sufixo de malha de alta polaridade** **Sufixo de malha de baixa polaridade** | Sufixos de nome de malha para identificar e agrupar a geometria ao usar o recurso Corresponder por nome. Sufixos disponíveis:<ul data-preserve-html="true"><li data-preserve-html="true"><strong>Malha poli baixa</strong>: sufixo para identificar malhas poli baixas na cena</li><li data-preserve-html="true"><strong>Malha poli alta</strong>: sufixo para identificar malhas poli altas na cena</li><li data-preserve-html="true"><strong>Ignorar faces traseiras</strong>: sufixo para identificar malhas que devem ser ignoradas por baker específicos (como a [Oclusão de ambiente da malha](../../bakers-settings/ambient-occlusion-from/ambient-occlusion-from-mesh.md))</li></ul>Para saber mais sobre a geometria correspondente, consulte: [Correspondência por nome](../../features/matching-by-name/matching-by-name.md) . |
|  |  |
| **Usar correção de inclinação** | Se habilitada, a direção do raio será calculada a partir da **Média Normal** ou da geometria original normal, dependendo da textura de entrada. Os valores de preto na textura usam o normal médio calculado enquanto os valores de branco usam o normal de malha original.*Não disponível no Substance Painter.* |
| **Mapa de Inclinação** | Caminho para o arquivo de textura usado para inclinar a projeção de raio. |
| **Inverter Correção De Inclinação** | Inverta a leitura da textura de entrada (preto se torna branco e branco se torna preto). |
