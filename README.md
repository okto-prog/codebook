<p align="center" style="margin: 24px;">
  <picture>
    <source media="(prefers-color-scheme: dark)" width="200" srcset=".assets/logo_dark.png">
    <source media="(prefers-color-scheme: light)" width="200" srcset=".assets/logo_light.png">
    <img alt="Oktoplus" width="200" src=".assets/logo_white.png">
  </picture>
</p>

<h1 align="center">
  Template Codebook Oktoplus
  <br>
  <a href="https://opensource.org/license/mit" target="_blank" rel="noopener noreferrer nofollow" style="display:inline-block"><img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="MIT License" style="max-width: 100%;"></a>
  <a href="https://github.com/okto-prog/codebook" target="_blank" rel="noopener noreferrer nofollow" style="display:inline-block"><img src="https://img.shields.io/badge/C%2B%2B-17-blue" alt="C++17" style="max-width: 100%;"></a>
  <a href="https://github.com/okto-prog/codebook"><img src="https://img.shields.io/github/stars/okto-prog/codebook?style=social" alt="GitHub stars"></a>
</h1>

<p align="left">
</p>

Notebook oficial de algoritmos e estruturas de dados em C++ da Oktoplus, equipe de Programação Competitiva do **CEFET-MG, Campus Leopoldina**, desenvolvido para dar suporte aos times em competições oficiais do ICPC.

Desenvolvido a partir do formato [Mashu-Codebook](https://github.com/Yuankai619/Mashu-Codebook). O repositório possui automação completa via GitHub Actions [`(compile.yml)`](./.github/workflows/compile.yml), gerando e atualizando o PDF final instantaneamente a cada push.

## Estrutura do Repositório

O projeto é estruturado de forma modular nas seguintes pastas:

```text
├── .fonts/             # Fontes TrueType (Consolas, Monaco) para o layout
├── .github/workflows/  # Workflow do GitHub Actions para compilação do PDF
├── arvore/             # HLD, LCA, Tree Hash e buscas em árvores
├── base/               # Templates C++, scripts de automação e testes
├── estruturaDeDados/   # SegTrees (Lazy, 2D, Persistente), BIT, Treap e DSU
├── flow/               # Fluxo máximo, corte mínimo e emparelhamento
├── geometria/          # Vetores, Convex Hull, Sweep Line e formas 2D/3D
├── grafo/              # Caminhos mínimos, SCC, pontes e conectividade
├── matematica/         # Teoria dos números, crivos, FFT e combinatória
├── ordenacao/          # Quicksort, Mergesort e ordenações lineares
├── outros/             # Implementações gerais e algoritmos diversos
├── PD/                 # Programação Dinâmica (Digit DP, SOS DP, Bitmask)
├── problemasEspeciais/ # Heurísticas (Simulated Annealing) e ad-hoc complexos
├── string/             # KMP, Z-function, Suffix Array e Palindrome Tree
├── codebook.tex        # Arquivo principal do LaTeX
├── content.tex         # Sumário e mapeamento dos códigos incluídos
└── codebook.pdf        # Documento final compilado para impressão
```


## Guia de Uso

Esta branch funciona como um esqueleto limpo e estruturado. Para começar a popular o seu caderno de algoritmos do zero, siga o passo a passo abaixo:

### Passo 1: Criar o Arquivo de Código
Identifique a pasta correspondente à área do algoritmo (ex: `estruturaDeDados/`, `grafo/`, `matematica/`) e crie o arquivo com a extensão `.cpp` (ou `.txt` para fórmulas).
* *Exemplo prático:* Para adicionar uma árvore segmentada, crie o arquivo em `estruturaDeDados/segTree.cpp`.

### Passo 2: Registrar no LaTeX (`content.tex`)
Abra o arquivo `content.tex` localizado na raiz do repositório, navegue até a seção temática do seu algoritmo e insira os comandos de mapeamento do LaTeX.

Você deve definir o título que aparecerá no índice (`\subsection`) e o caminho do arquivo (`\lstinputlisting`):

```latex
\subsection{Segment Tree Iterativa}
\lstinputlisting{estruturaDeDados/segTree.cpp}
```

> **Atenção com Espaços no Nome:** Se o seu arquivo possuir espaços no nome (ex: Sparse Table.cpp), o LaTeX exige que o caminho seja envolvido por aspas simples dentro das chaves: `\lstinputlisting{estruturaDeDados/'Sparse Table.cpp'}`

### Diretrizes e Boas Práticas

Para manter o codebook conciso, padronizado e legível no papel, sugerimos seguir estas diretrizes ao adicionar ou editar um algoritmos:

1. **Siga o Código Base:** Sempre utilize a estrutura padrão contida em `base/base.cpp` como ponto de partida para os seus arquivos. Isso garante que todas as implementações compartilhem dos mesmos includes essenciais, macros utilitárias e otimizações de I/O (`fastio`), mantendo o comportamento do código previsível e padronizado.

2. **Defina a Complexidade:** Inclua obrigatoriamente um comentário curto na primeira linha do arquivo indicando a complexidade de tempo e espaço. (ex: // Complexidade: O(N * logN) tempo / O(N) espaço).

3. **Otimize a Formatação para Impressão:** Como o objetivo do codebook é ser uma consulta impressa em colunas, formate o código para que ele seja denso e legível. Evite quebras de linha excessivas, remova linhas em branco redundantes e evite chaves soltas ocupando uma linha inteira sem necessidade. Evite escrever linhas longas para que o LaTeX não quebre seu código de forma estranha no PDF.

4. **Garantia de Accepted (AC):** Nunca envie um algoritmo para o repositório baseado apenas em teoria. O código deve ser testado e validado em problemas de juízes online (Beecrowd, Codeforces, AtCoder, etc.) antes do commit.

## Integrantes e Contribuidores

O desenvolvimento e a manutenção deste projeto são realizados pelos coordenadores e membros da equipe Oktoplus.
Agradecemos ao CEFET-MG, pelo apoio institucional e fomento ao projeto de Programação Competitiva.
