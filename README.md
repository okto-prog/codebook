<p align="center" style="margin: 24px;">
  <picture>
    <source media="(prefers-color-scheme: dark)" width="200" srcset=".assets/logo_dark.png">
    <source media="(prefers-color-scheme: light)" width="200" srcset=".assets/logo_light.png">
    <img alt="Oktoplus" width="200" src=".assets/logo_white.png">
  </picture>
</p>

<h1 align="center">
  Codebook Oktoplus
  <br>
  <a href="https://opensource.org/license/mit" target="_blank" rel="noopener noreferrer nofollow" style="display:inline-block"><img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="MIT License" style="max-width: 100%;"></a>
  <a href="https://github.com/okto-prog/codebook" target="_blank" rel="noopener noreferrer nofollow" style="display:inline-block"><img src="https://img.shields.io/badge/C%2B%2B-17-blue" alt="C++17" style="max-width: 100%;"></a>
  <a href="https://github.com/okto-prog/codebook"><img src="https://img.shields.io/github/stars/okto-prog/codebook?style=social" alt="GitHub stars"></a>
  <br>
  <a href="https://github.com/okto-prog/codebook/actions/workflows/compile.yml" target="_blank" rel="noopener noreferrer nofollow"><img src="https://img.shields.io/github/actions/workflow/status/okto-prog/codebook/compile.yml?style=for-the-badge&logo=github&label=Compilador" alt="Compilar Codebook"></a>
  <a href="https://github.com/okto-prog/codebook/blob/main/codebook.pdf" target="_blank"><img src="https://img.shields.io/badge/📄_PDF_Codebook-Abrir-blue?style=for-the-badge"></a>
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

##  Integrantes e Contribuidores

O desenvolvimento e a manutenção deste projeto são realizados pelos coordenadores e membros da equipe Oktoplus.
Agradecemos ao CEFET-MG e à Diretoria de Extensão e Desenvolvimento Comunitário (DEDC) pelo apoio institucional e fomento ao projeto de Programação Competitiva.
