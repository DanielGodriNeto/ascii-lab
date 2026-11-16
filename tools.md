# tools.md — Geradores/ferramentas de ASCII locais (pesquisa 2026-11-15)

Dados de estrelas/commits: API do GitHub em 2026-11-15. Instalação no Windows NÃO verificada, salvo onde indicado.
Legenda: ⭐ = melhor caso | ⚠️ = cuidado

## Projeto relacionado
Cubo de Rubik 3D em ASCII, rotacionável. Ver "Melhores casos" no fim.

## 1. Imagem / vídeo / webcam → ASCII
| Ferramenta | Lang | Estrelas | Último commit | Notas |
|---|---|---|---|---|
| ⭐ [chafa](https://github.com/hpjansson/chafa) | C | 5404 | 2026-11-15 (v1.18.3) | Melhor qualidade: truecolor, braille/blocos, sixel/kitty/iTerm2, GIF animado. Sem webcam. Release só com fonte; binário Windows/scoop/winget não verificado |
| ⭐ [tplay](https://github.com/maxcurzi/tplay) | Rust | 703 | 2026-08-31 | Melhor CLI para vídeo, webcam e GIF. Windows não verificado |
| [viu](https://github.com/atanunq/viu) | Rust | 3314 | 2025-12-15 | Único com `.exe` oficial (viu-x86_64-pc-windows-msvc.exe). Blocos + kitty/sixel, GIF, sem webcam |
| [tiv](https://github.com/stefanhaustein/TerminalImageViewer) | C++ | 1688 | 2026-11-03 | Blocos unicode 24-bit, só imagens |
| [libcaca / img2txt](https://github.com/cacalabs/libcaca) | C | 703 | 2026-08-14 | Dithering, exporta HTML/ANSI. Pacote Cygwin |
| [artem](https://github.com/FineFindus/artem) | Rust | 348 | 2025-06-15 | Zip Windows nos releases (v3.0.0, 2024) |
| [jp2a (fork Talinx)](https://github.com/Talinx/jp2a) | C | 105 | 2025-12-16 | Mínimo, JPEG/PNG |
| ⚠️ [ascii-image-converter](https://github.com/TheZoraiz/ascii-image-converter) | Go | 3573 | 2024-04-14 | Popular mas parado (release 2022). Evitar |
| [ratatui-image](https://github.com/benjajaja/ratatui-image) | Rust | 419 | 2026-10-18 | Biblioteca p/ TUIs, não CLI |

Novos (só trechos de busca, não inspecionados): [TermiCam](https://pkg.go.dev/github.com/Megge06/TermiCam) (Go, webcam+gravação, precisa FFmpeg), [ascii-chat](https://github.com/zfogg/ascii-chat) (C, 203★, videochat no terminal), [DotFrame](https://github.com/NyxLumen/DotFrame) (webcam→ASCII no navegador, exporta WebM).

## 2. Texto (banners) e diagramas
| Ferramenta | Lang | Estrelas | Último push | Notas |
|---|---|---|---|---|
| ⭐ [cfonts](https://github.com/dominikwilkowski/cfonts) | Rust/JS | 1911 | 2026-11 | Banners com cor e gradiente. `npm i -g cfonts` |
| ⭐ [figlet.js](https://github.com/patorjk/figlet.js) | JS | 3045 | 2026-10 | Muitas fontes, boa API. `npm i figlet` |
| ⭐ [terminaltexteffects](https://github.com/ChrisBuilds/terminaltexteffects) | Py | 4305 | hoje | Efeitos animados de texto, o mais ativo. `pip install terminaltexteffects` |
| [oh-my-logo](https://github.com/shinshin86/oh-my-logo) | TS | 1606 | 2026-05 | Logos com gradiente, `npx oh-my-logo` |
| [pyfiglet](https://github.com/pwaller/pyfiglet) | Py | 1595 | 2026-08 | Figlet em Python |
| [gradient-string](https://github.com/bokub/gradient-string) | JS | 551 | 2026-07 | Biblioteca, não CLI |
| ⭐ [asciiflow](https://github.com/lewish/asciiflow) | TS | 5999 | 2026-07 | Melhor editor grátis de diagramas. Web app (offline só se hospedar) |
| [MonoSketch](https://github.com/tuanchauict/MonoSketch) | Kotlin | 1826 | 2026-10 | Mais parecido com Monodraw. Web app |
| [mermaid-ascii](https://github.com/AlexanderGrooff/mermaid-ascii) | Go | 1627 | 2026-10 | Mermaid → ASCII, bom p/ docs e saída de LLM |
| [svgbob](https://github.com/ivanceras/svgbob) | Rust | 4239 | 2026-04 | Inverso: ASCII → SVG. `cargo install svgbob_cli` |
| [ASCII Draw (Nokse22)](https://github.com/Nokse22/ascii-draw) | — | 694 | 2026-07 | GNOME/GTK, ruim p/ Windows |
| [play.core](https://github.com/ertdfgcvb/play.core) | JS | 545 | 2026-04 | Animação ASCII criativa |
| [YuzuDraw](https://www.hnshowcase.com/post/47414536/yuzudraw-visual-editor-for-ascii-diagrams-with-token-efficie) | — | ? | 2026 | Show HN, editor de diagramas c/ integração de agente |
| ⚠️ figlet (C) / toilet / Graph-Easy | — | — | 2023 / 2024 / 2010 | Parados; figlet continua referência |

## 3. IA local e shaders
- **Veredito:** LLM local desenha ASCII tosco (só coisas simples: pelicano, gato). Para ficar bonito: gerar/ter imagem ou cena 3D e converter por algoritmo/shader.
- ⭐ [three.js AsciiEffect](https://threejs.org/docs/pages/AsciiEffect.html): addon oficial, cena 3D → ASCII em tempo real.
- [pmndrs ASCIIEffect](https://pmndrs.github.io/postprocessing/public/docs/class/src/effects/ASCIIEffect.js~ASCIIEffect.html): postprocessing (não combina com efeitos de convolução).
- [Codrops "Efecto" (jan/2026)](https://tympanus.net/codrops/2026/01/04/efecto-building-real-time-ascii-and-dithering-effects-with-webgl-shaders): tutorial GLSL.
- [p5.asciify](https://discourse.processing.org/t/p5-asciify-apply-real-time-ascii-conversion-to-your-favorite-webgl-p5-js-sketches-instantly/44893): p5.js.
- ComfyUI (nível hobby, só vistos em agregadores): [EllangoK AsciiArt](https://www.runcomfy.com/comfyui-nodes/ComfyUI-post-processing-nodes/AsciiArt), [LamEmil ASCIIArtNode](https://awesome.ecosyste.ms/projects/github.com%2FLamEmil%2FComfyUI_ASCIIArtNode), [color-ascii-art-node](https://www.comfyonline.app/comfyui-nodes/ComfyUI-color-ascii-art-node).
- LLMs: Qwen3.6-35B-A3B (llama.cpp Q4_K_M ~22 GB) e Gemma 4 são os melhores palpites, mas só há testes anedóticos ([post](https://dev.to/jtorchia/qwen36-35b-a3b-runs-on-my-laptop-and-draws-better-than-claude-opus-47-bh5), [HF](https://huggingface.co/SerialKicked/ModelTestingBed/discussions/4)). Fine-tunes tipo PetarKal/Qwen3-4B-ascii-art: sem evidência de qualidade.
- Datasets: [mrzjy/ascii_art_generation_140k](https://huggingface.co/datasets/mrzjy/ascii_art_generation_140k) (Apache-2.0; feito por conversor, então ensina a imitar conversor), [retro-ascii-art-v1](https://huggingface.co/datasets/jdpressman/retro-ascii-art-v1) (CC0).
- Benchmarks: [ASCIIEval](https://arxiv.org/html/2410.01733v2) (reconhecimento), [ASCIIBench](https://arxiv.org/abs/2512.04125v1) (geração; sem leaderboard confiável).
- [ascii-flux-v1](https://huggingface.co/martintomov/ascii-flux-v1): LoRA do Flux que gera imagem estilo ASCII (não texto).

## Lacunas da pesquisa
Instalação no Windows não verificada (chafa, tplay, tiv); Reddit/HN/X pouco cobertos, nenhum post viral de 2025-26 achado; nenhuma comparação independente recente; nada foi executado.

## ⭐ Melhores casos (resumo)
- Imagem/GIF: **chafa**. Vídeo/webcam: **tplay**. Windows sem dor: **viu**.
- Banner de texto: **cfonts** ou **figlet.js**. Efeito animado: **terminaltexteffects**.
- Diagrama: **asciiflow** (ou MonoSketch).
- 3D interativo/rotacionável: **three.js AsciiEffect** (ver abaixo).
- IA: converter imagem por algoritmo; LLM só p/ desenho simples.

## Projeto: Cubo de Rubik 3D rotacionável em ASCII
Viável. Duas rotas:
1. ⭐ Web: three.js + AsciiEffect + OrbitControls. 27 cubies com adesivos coloridos, arrastar com o mouse gira o cubo, teclas giram as camadas. Menos código, 3D real.
2. Terminal: renderizador próprio (Python/Rust) com matrizes de rotação e z-buffer, teclas para girar. Mais controle, mais trabalho.
Limite: ASCII tem resolução baixa, as cores dos adesivos exigem modo colorido (o AsciiEffect tem opção `color`).

## Resultado: rubik-ascii.html (2026-11-16)
Arquivo pronto: `rubik-ascii.html` (abrir no navegador, precisa internet p/ CDN do three.js). Arrastar gira, roda dá zoom, teclas U/D/L/R/F/B (Shift = inverso), Embaralhar/Resetar, sliders de resolução e velocidade, troca de caracteres, cores on/off.
Nota: AsciiEffect com fundo escuro precisa `invert:true`, senão partes claras viram espaço. Interação testada só visualmente (painel estático).

## Resultado: rook-ascii.html (2026-11-16)
Torre de xadrez (LatheGeometry + 4 ameias) num tabuleiro 8x8, mesma base do cubo. Setas movem uma casa por toque (limitadas ao tabuleiro, interpolação suave), mostra a casa atual (a1..h8). Arrastar gira a câmera.

## Repo: ascii-lab
Reúne rubik-ascii.html, rook-ascii.html, tools.md e README. Só local por enquanto (sem GitHub).
