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

O link **Baixar** aponta para o pacote da release quando há uma distribuição
pronta; nos projetos sem release, aponta para o zip do código do branch
principal. Confira no README de cada jogo se o download é código-fonte ou
um pacote para instalar. As distribuições experimentais da conta EoTutts
listadas abaixo são para **R36S RK3326/Linux ARM64**, com requisitos, créditos
e SHA-256 nos respectivos repositórios; não são pacotes para GA36/ARMv7.

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
- [Embers of Yulan](https://github.com/gogabs/embers-of-yulan) — Sobrevivência à
  beira de um rio assombrado: de dia, procure comida e material no campo, no
  bambuzal e na margem; de noite, os jiangshi, mortos que andam aos pulos, saem
  do rio em ondas e vêm até a sua fogueira. Som 3D, com um "tic" no centro para
  mirar sem fone. Um único jogo salvo e uma vida só. Protótipo, versão 0.7.2, sem
  release ainda.
  [Baixar](https://github.com/gogabs/embers-of-yulan/archive/refs/heads/main.zip)
- [Dead vs. Alive](https://github.com/gogabs/dead-vs-alive) — Sobreviva às
  ondas de zumbis ouvindo de onde eles vêm, sala por sala, trocando de arma a
  cada onda. Um bipe na direção do zumbi na mira diz a distância, então dá para
  jogar sem fone. Sons do Swamp, do Aprone. Versão 0.1.0, sem release ainda.
  [Baixar](https://github.com/gogabs/dead-vs-alive/archive/refs/heads/main.zip)
- [Rolê](https://github.com/gogabs/luma-role) — Patinação urbana sem parar: você
  patina sozinho, cada obstáculo avisa em três batidas com um som próprio e
  você pula, freia, pega rampa, desliza no corrimão, desce escadas e faz curvas,
  além das manobras no ar. O combo faz a música ganhar camadas e três quedas
  encerram a corrida. Jogável sem estéreo e com pixel art. Protótipo, versão
  0.1.0, sem release ainda.
  [Baixar](https://github.com/gogabs/luma-role/archive/refs/heads/main.zip)

- [Pokémon ShowUp](https://github.com/EoTutts/pokemon-showup) — Batalhas
  Pokémon com times de seis, IA, dois jogadores no mesmo console, partidas em
  rede e campanha Jornada de nove regiões. Versão 0.5.0+r36s-audio.20261012,
  distribuição experimental para R36S ARM64.
  [Baixar](https://github.com/EoTutts/pokemon-showup/releases/download/v0.5.0-r36s-audio.20261012-distribution.20261106/pokemon-showup-linux-arm64.zip)
- [Port Mondes](https://github.com/EoTutts/port-mondes) — Porte acessível do
  RPG Port Mondes, com exploração, combates por turnos, inventário, magia e
  aventuras em português, inglês e francês. Versão 0.1.0, distribuição
  experimental para R36S ARM64.
  [Baixar](https://github.com/EoTutts/port-mondes/releases/download/v0.1.0-distribution.20261106/port-mondes-linux-arm64.zip)
- [Galope](https://github.com/EoTutts/galope) — Corrida sem fim a cavalo:
  salte obstáculos e escape dos cães, com pistas sonoras posicionais,
  velocidade crescente e gráficos opcionais. Versão 1.0.0, distribuição
  experimental para R36S ARM64.
  [Baixar](https://github.com/EoTutts/galope/releases/download/v1.0.0-distribution.20261106/galope-linux-arm64.zip)

## Apps

- [Vinyl](https://github.com/gogabs/vinyl) — Player de audiolivros e música
  com menus falados, pelo mpv: retoma cada livro de onde parou, marcadores,
  velocidade sem mudar o tom e timer para dormir. Lê as pastas `audiolivros` e
  `musica` do cartão. Versão 0.1.0, sem release ainda.
  [Baixar](https://github.com/gogabs/vinyl/archive/refs/heads/main.zip)

## Como instalar um jogo

Nos pacotes compilados, extraia o ZIP completo e copie a pasta que contém o
`game.json` para `a11y/games/` na partição EASYROMS do cartão. O nome da pasta
deve ser o `id` do manifesto. Também é possível enviar o ZIP pela opção
**Instalar jogo** da Página no PC do Luma. Feche o jogo antes de atualizar e
preserve `a11y/saves/`. Os jogos .NET precisam do runtime compartilhado do
Luma; Port Mondes inclui Python 3.8 privado. Requisitos e estado de validação
ficam no README de cada distribuição.

Nos jogos distribuídos como código-fonte, siga as instruções de build ou o
`instalar.sh` do próprio projeto. Com o Mage
Core clonado ao lado do repositório do jogo, rode `./instalar.sh` e o jogo
aparece na lista sozinho. Os detalhes de cada um estão no README do
repositório. Para rodar no PC (Windows), use o Mage:
`python mage.py run <pasta do jogo>`.

## Contribuir

Achou um jogo ou ferramenta para o Luma que falta aqui? Abra um pull request
com uma linha na seção certa, no mesmo formato: nome com link, um travessão e
uma frase dizendo o que é, e o link de download da release, se houver.
