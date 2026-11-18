# Catálogo de partituras do Clavi

Partituras de piano em MusicXML (`.mxl`) para o catálogo pesquisável do app **Clavi**, que ensina a tocar
piano lendo partitura. Este repositório só hospeda os arquivos (via GitHub Pages); o app lê daqui.

- `indice.json`: lista com título (`t`), compositor (`c`), nível (`n`: 0 Fácil, 1 Médio, 2 Desafio),
  número de compassos (`m`) e `h: 1` quando usa as duas mãos. O arquivo de cada item fica em `p/<i>.mxl`.
- 7.551 partituras, cerca de 51 MB.

## De onde vêm

Seleção do **PDMX: A Large-Scale Public Domain MusicXML Dataset for Symbolic Music Processing**,
de Phillip Long, Zachary Novack, Julian McAuley e Taylor Berg-Kirkpatrick (UC San Diego),
publicado no Zenodo sob a licença [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/):
https://doi.org/10.5281/zenodo.15571083 · artigo: https://arxiv.org/abs/2409.10831

As partituras do PDMX foram publicadas no MuseScore como domínio público ou CC0. Daqui foram usadas só as do
subconjunto `no_license_conflict`, com uma única parte de piano e uma versão por música, e **só de
compositores que morreram até 1954 ou de músicas tradicionais/anônimas** (arranjos de músicas pop, de games
e de filmes ficaram de fora, porque a música original continua protegida). Os arquivos `.mxl` não foram
alterados; os nomes foram trocados para um id curto e os títulos/compositores do índice foram limpos.

O filtro é automático (por texto). Se alguma partitura aqui não deveria estar, abra uma issue que ela sai.

Gerado pelo script `scripts/catalogo/gerar-catalogo.mjs` do repositório do app.
