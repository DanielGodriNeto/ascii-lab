# ascii-lab

Experimentos de ASCII em 3D no navegador (three.js + `AsciiEffect`). Basta abrir o HTML; precisa de internet para carregar o three.js pela CDN.

## Páginas

| Arquivo | O que é | Controles |
|---|---|---|
| `rubik-ascii.html` | Cubo de Rubik 3D | Arrastar gira o cubo, roda do mouse dá zoom, teclas `U D L R F B` giram camadas (com `Shift` ao contrário), botões Embaralhar/Resetar |
| `rook-ascii.html` | Torre de xadrez num tabuleiro 8x8 | Setas `← ↑ → ↓` movem a torre uma casa por toque, arrastar gira a câmera, roda dá zoom |
| `rook-solo-ascii.html` | Só a torre, sem tabuleiro | Setas `← →` giram a torre, `↑ ↓` inclinam, arrastar gira a câmera, roda dá zoom |

Todas têm sliders de resolução, troca de conjunto de caracteres, cores on/off e "girar sozinho".

## Notas

`tools.md` reúne a pesquisa (2026-11-15) de geradores de ASCII locais, com os melhores casos destacados.

## Detalhe técnico

Com fundo escuro o `AsciiEffect` precisa de `invert: true`, senão as partes claras viram espaço.
