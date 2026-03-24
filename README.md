# ToddyMarkDown VS Code Extension

Esta é a extensão oficial para suporte à linguagem **ToddyMarkDown** (`.tmd`) no Visual Studio Code.

## O que é ToddyMarkDown?
ToddyMarkDown é uma extensão semântica do Markdown tradicional, focada em escrita editorial rica, ensaios estruturados e documentação técnica avançada. Ele permite diagramar elementos visuais sofisticados (citações destacadas, linhas do tempo, imagens laterais "abraçadas" pelo texto) usando Blocos Especiais (`|>` e `<|`), mantendo a leveza de um arquivo de texto puro.

Para ler a especificação completa, consulte a [Especificação do ToddyMarkDown](../_docs/tmd-spec/tmd-spec-v1.4.md).

## Como Instalar em Desenvolvimento
1. Abra este diretório (`tmd-vscode-extension`) no VS Code.
2. Pressione `F5` para abrir uma nova janela do VS Code ("Extension Development Host") com a extensão carregada.
3. Crie ou abra um arquivo com extensão `.tmd` para verificar o syntax highlighting customizado.

## Tabela de Tokens e Cores
A extensão inclui um tema dark customizado (`ToddyMarkDown Theme`) que mapeia semanticamente as categorias de syntax highlight:

| Símbolo / Estrutura | Significado | Cor (vs-dark) |
| --- | --- | --- |
| `\|>` / `<\|` | Delimitador de bloco especial | Magenta (`#ff4fd8`) |
| `/>` / `<\\` | Delimitador de bloco literal | Magenta (`#ff4fd8`) |
| `!`, `@`, `##`, `+`, `?`... | Token do bloco de conteúdo | Dourado (`#d9a441`) |
| `*>`, `*<wrap`, etc. | Modos de imagem | Dourado (`#d9a441`) |
| `[Título]` | Título opcional de blocos | Laranja (`#ff9b42`) |
| `#` / `##` / `###` | Headings Markdown | Tons de Azul |
| `-` | Marcador de Lista Markdown | Dourado Claro (`#e3c77a`) |
| `>` | Citação simples Markdown | Vermelho (`#e05757`) |
| `---` | Metadados / Frontmatter Keys | Verde (`#a4cd54`) |
