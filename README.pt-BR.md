# VectorCraft — documentação em português do Brasil (pt-BR)

**Ilustração vetorial; uma reimplementação open-source e clean-room do Adobe Illustrator, reconstruída em Rust puro.**

Feito em Rust puro, funciona nativamente em macOS, Windows e Linux e também no navegador via WebAssembly.

## Recursos

- Familiar: layout, ferramentas, menus, painéis e atalhos do Illustrator — Pen, Seleção Direta, Pathfinder e mais.
- Rápido: renderização SIMD multithread fora da thread da UI — 20.000 formas em ~27 ms.
- Robusto: booleanos de curva exatos (sem “cannot perform operation”) e undo ilimitado via estrutura copy-on-write.
- Aberto: formato nativo documentado (.vectorcraft, JSON), SVG de primeira classe e compatibilidade com PDF.

## Português do Brasil

Este fork detecta automaticamente pt-BR pelo locale do sistema — sem configuração extra.

PR #384 já foi MESCLADO no upstream — a interface em pt-BR é oficial.

## A suíte ArtCraft

A ArtCraft é um conjunto de 7 aplicativos open-source que reimplementam, de forma clean-room e em Rust puro, as ferramentas de criação da Adobe — nativos para macOS, Windows e Linux, com a mesma interface no navegador via WebAssembly:

| Aplicativo | Propósito | Reimplementação de |
|---|---|---|
| PhotoCraft | Edição de imagens | Adobe Photoshop |
| FilmCraft | Edição de vídeo, cor e som | Adobe Premiere Pro |
| LightCraft | Biblioteca de fotos e revelação RAW | Adobe Lightroom |
| EffectCraft | Motion graphics e efeitos visuais | Adobe After Effects |
| PrintCraft | Workbench de PDF | Adobe Acrobat |
| DesignCraft | Layout de página e publicação | Adobe InDesign |
| VectorCraft | Ilustração vetorial | Adobe Illustrator |

- Site: <https://getartcraft.com> · Discord: <https://discord.gg/artcraft>

## Este fork

Adiciona **leitura desta documentação em português do Brasil** e, no código, a **tradução pt-BR da interface** — sem alterar nada do comportamento do aplicativo original.


## Instalar no Linux (x86_64)

Baixe o tarball da release e extraia (sem precisar de sudo):

```bash
wget https://github.com/storytold/vectorcraft/releases/download/v0.4.0/vectorcraft-0.4.0-linux-x86_64.tar.gz
mkdir -p ~/Programas/vectorcraft
tar -xzf vectorcraft-0.4.0-linux-x86_64.tar.gz -C ~/Programas/vectorcraft --strip-components=1
~/Programas/vectorcraft/bin/vectorcraft
```

> Consulte a página de releases do repositório upstream para a versão e o nome do asset atuais.

## Compilar do código

```bash
git clone https://github.com/storytold/<repositorio-upstream>.git
cd <repositorio-upstream>
# (opcional, para as fontes CJK do release) export CRAFT_FONTS_DIR=~/craft-fonts CRAFT_FONTS_REQUIRED=1
cargo build --release
```

## Comunidade

Suporte, feedback e novidades da suíte no Discord: <https://discord.gg/artcraft>.

---

Documentação original (inglês): [`README.md`](README.md).

