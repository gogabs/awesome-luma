# Awesome Luma [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> Jogos e ferramentas acessíveis para o console portátil R36S, jogáveis só com
> som e fala, por pessoas cegas e com baixa visão.

O **Luma** deixa o R36S (ArkOS 2.0) usável sem enxergar a tela: uma lista de
jogos falada, atalhos de sistema com retorno falado e vozes em português. Tudo
o que está aqui roda nele, e quase tudo roda também no PC.

*Awesome Luma is a curated list of accessible audio games and tools for the
R36S handheld running Luma/ArkOS. Everything is in Brazilian Portuguese.*

## Sumário

- [Sobre os downloads](#sobre-os-downloads)
- [Engine](#engine)
- [Jogos](#jogos)
- [Apps](#apps)
- [Como instalar um jogo](#como-instalar-um-jogo)
- [Contribuir](#contribuir)

## Sobre os downloads

Nenhum dos jogos tem release publicada no GitHub ainda. Por enquanto, o link
**Baixar** de cada item é o zip do código atual do branch principal, gerado
pelo GitHub na hora. Ele tem o `instalar.sh` e a cópia da biblioteca
`r36s_a11y`, e serve para instalar no console ou rodar no PC. Quando um jogo
ganhar release, o link passa a apontar para ela.

## Engine

- [Mage](https://github.com/gogabs/mage) — A engine dos jogos acessíveis do
  R36S. Cria, roda, confere e exporta jogos pela linha de comando ou por um
  editor no navegador: um zip para o cartão do R36S e um `.exe` para Windows
  que abre sem instalar nada. Só precisa de Python 3.7 ou mais novo. Licença
  MIT. Sem release ainda.
  [Baixar](https://github.com/gogabs/mage/archive/refs/heads/main.zip)
- [Mage Core](https://github.com/gogabs/r36s-a11y-sdk) (repositório
  `r36s-a11y-sdk`) — O núcleo do Mage: o contrato entre jogos e a plataforma e
  as bibliotecas-ponte em Python (`r36s_a11y`), Go, LÖVE e C#, que leem o
  controle, falam pelo Speech Dispatcher e tocam som 3D pela OpenAL sem
  atropelar o leitor de tela. Licença MIT. Sem release ainda.
  [Baixar](https://github.com/gogabs/r36s-a11y-sdk/archive/refs/heads/main.zip)
  - [Contrato dos jogos](https://github.com/gogabs/r36s-a11y-sdk/blob/main/docs/contrato.md)
  - [Gráficos opcionais](https://github.com/gogabs/r36s-a11y-sdk/blob/main/docs/graficos.md)
  - [Áudio em cada linguagem](https://github.com/gogabs/r36s-a11y-sdk/blob/main/docs/audio-por-linguagem.md)

## Jogos

- [Stelar Flow](https://github.com/gogabs/stelar-flow) — Você é uma estrela:
  funda os elementos numa grade hexagonal, do hidrogênio ao ferro, antes que o
  ferro tome conta. Por turnos, com quatro finais possíveis. Versão 0.3.0, sem
  release ainda.
  [Baixar](https://github.com/gogabs/stelar-flow/archive/refs/heads/main.zip)
- [Solitários](https://github.com/gogabs/r36s-solitaire) (repositório
  `r36s-solitaire`) — Três jogos num repositório só. Sem release ainda.
  [Baixar](https://github.com/gogabs/r36s-solitaire/archive/refs/heads/main.zip)
  - [Paciência](https://github.com/gogabs/r36s-solitaire/tree/main/paciencia) —
    Klondike, FreeCell e Spider, com as cartas faladas.
  - [Campo Minado](https://github.com/gogabs/r36s-solitaire/tree/main/campo-minado) —
    Abra as casas sem mina, ouvindo os números em volta. Fácil, médio e difícil.
  - [Sudoku](https://github.com/gogabs/r36s-solitaire/tree/main/sudoku) —
    Preencha a grade de 1 a 9 sem repetir, com grades sorteadas.
- [Comes e Bebes](https://github.com/gogabs/comes-e-bebes) — Toque uma
  lanchonete no seu ritmo: faça as compras, atenda as mesas, cozinhe sem
  queimar e limpe tudo no fim do dia, pelas quatro estações. Primeiro
  protótipo, versão 0.1.0, sem release ainda.
  [Baixar](https://github.com/gogabs/comes-e-bebes/archive/refs/heads/main.zip)
- [Rio Abaixo](https://github.com/gogabs/rio-abaixo) — Para dois, com um fone:
  o piloto rema a canoa e o vigia, ouvindo só o rio à frente, guia pela voz.
  Versão 0.2.0, sem release ainda.
  [Baixar](https://github.com/gogabs/rio-abaixo/archive/refs/heads/main.zip)
- [Dead vs. Alive](https://github.com/gogabs/dead-vs-alive) — Sobreviva às
  ondas de zumbis ouvindo de onde eles vêm, sala por sala, trocando de arma a
  cada onda. Um bipe na direção do zumbi na mira diz a distância, então dá para
  jogar sem fone. Sons do Swamp, do Aprone. Versão 0.1.0, sem release ainda.
  [Baixar](https://github.com/gogabs/dead-vs-alive/archive/refs/heads/main.zip)

## Apps

- [Vinyl](https://github.com/gogabs/vinyl) — Player de audiolivros e música
  com menus falados, pelo mpv: retoma cada livro de onde parou, marcadores,
  velocidade sem mudar o tom e timer para dormir. Lê as pastas `audiolivros` e
  `musica` do cartão. Versão 0.1.0, sem release ainda.
  [Baixar](https://github.com/gogabs/vinyl/archive/refs/heads/main.zip)

## Como instalar um jogo

Com o console montado pelo Luma, cada jogo traz um `instalar.sh`: com o Mage
Core clonado ao lado do repositório do jogo, rode `./instalar.sh` e o jogo
aparece na lista sozinho. Os detalhes de cada um estão no README do
repositório. Para rodar no PC (Windows), use o Mage:
`python mage.py run <pasta do jogo>`.

## Contribuir

Achou um jogo ou ferramenta para o Luma que falta aqui? Abra um pull request
com uma linha na seção certa, no mesmo formato: nome com link, um travessão e
uma frase dizendo o que é, e o link de download da release, se houver.
