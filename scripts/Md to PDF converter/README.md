---
source-git-commit: a517442244806bc6aef0f5bfb165c5d4f67341be
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---
# Markdown para o conversor de PDF

Essa pasta contém um script de pré-processamento e conversão para gerar versões de PDF das páginas de documentação a partir desse repositório.

## Por que isso existe

Os arquivos de origem da documentação usam a sintaxe de redução específica da plataforma Adobe (blocos acordeão, chamadas de alerta e extensões de atributo de imagem) que as ferramentas de redução padrão não entendem. Este script normaliza essa sintaxe e converte o arquivo em um PDF usando [md-to-pdf](https://github.com/simonhaenisch/md-to-pdf), enquanto também compacta imagens para manter o tamanho do arquivo de saída gerenciável.

## Pré-requisitos

- [Node.js](https://nodejs.org/) (v18 ou posterior)
- As dependências já estão instaladas em `node_modules/`. Se precisar reinstalá-los, execute o `npm ci` a partir desta pasta.

## Uso

Execute o script a partir da **raiz do repositório**, passando o caminho para o arquivo de marcação que você deseja converter:

```
node "scripts/Md to PDF converter/preprocess-for-pdf.js" <path/to/file.md>
```

**Exemplo:**

```
node "scripts/Md to PDF converter/preprocess-for-pdf.js" help/substance-3d-general/openpbr/openpbr-overview.md
```

O PDF é gravado no **mesmo diretório do arquivo de origem**. Os arquivos temporários criados durante a conversão (`*.pdf-ready.md` e `_pdf-images/`) são excluídos automaticamente em caso de êxito. Se a conversão falhar, eles serão deixados no lugar para ajudar na depuração.

## O que o script faz

| Sintaxe de origem | saída de PDF |
|---|---|
| `+++Title` / `+++` blocos acordeão | Título `#####` com conteúdo sempre visível |
| `>[!NOTE]` chamadas de alerta | blockquote padrão com negrito **Observação:** prefixo |
| Atributos de imagem de `![](path){width="N"}` | Marca `<img>` preservando a largura especificada |
| Links de imagens de markdown para `.pdf` arquivos | Removido (referências de download automático somente para a Web) |
| `hold:` chave do frontmatter | Removido (metadados somente de plataforma) |
| Todas as imagens | Redimensionado para o máximo de 1200 px de largura, codificado novamente como JPEG com 80% de qualidade |
| Todas as tabelas | Bordas e fundos removidos por meio de CSS injetado |
