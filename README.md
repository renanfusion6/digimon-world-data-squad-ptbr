# Digimon World Data Squad — Tradução PT-BR (v0.9 beta)

Tradução de fã do **Digimon World Data Squad** (PlayStation 2, versão americana) para o português do Brasil.

Aqui você encontra só o **patch** (`.xdelta`), que guarda apenas as diferenças em relação ao jogo original. **Nenhum arquivo do jogo é distribuído aqui.** Você precisa da sua própria cópia (ISO) da versão americana.

---

## O que está traduzido

- **História completa**: os 11 capítulos, eventos secundários, conversas na base DATS, tutoriais, enigmas e quizzes.
- **Menus e sistema**: cartão de memória, lojas, opções, mensagens de batalha.
- **Itens**: nomes, efeitos e descrições dos 302 itens.
- **Habilidades e comandos de suporte**: nomes e descrições.
- **Golpes**: descrições traduzidas. Os nomes dos golpes ficam em inglês, como no anime e na versão americana (ex.: *Pepper Breath*, *D Crescent Mirage*).
- **Enciclopédia** (145 Digimon), **condições de evolução** e **nomes de mapa**.
- **Telas desenhadas em imagem**:
  - tela de título;
  - menu principal;
  - cabeçalhos das telas e abas;
  - barra de botões ("Escolher", "Voltar", "Pronto"...);
  - Sim/Não;
  - mapa de evolução;
  - equipe;
  - roleta de batalha (Ação, Defesa, Fuga, Suporte);
  - resultado da batalha.
- **Acentos**: a fonte do jogo ganhou as letras acentuadas do português (á, ã, ç, é, õ...).

Ficam como no original, de propósito: nomes de personagens e de Digimon, nomes de golpes, siglas de atributo (HP, STR, DEF...) e créditos.

## Ainda em inglês (próximas versões)

- Estados no cartão da batalha (Poison, Sleep, Panic, Anger...).
- "MESSAGE" no topo da caixa de fala.
- Logos animados ("Evolution", "Game Over", "Now Loading").
- Miniaturas de prévia no menu principal.
- Alguns rótulos pequenos (Name, LV, RANK).

Encontrou um erro, uma frase cortada ou algo em inglês fora desta lista? Abra uma *Issue* com um print e o local do jogo.

---

## Do que você precisa

1. A ISO **americana** do jogo: **Digimon World Data Squad (USA)**, código **SLUS-21598**.
2. O patch: `Digimon World - Data Squad PT-BR v0.9.xdelta` (veja em *Releases*).
3. Um programa que aplique patches xdelta (opções abaixo).

### Confira se a sua ISO é a certa

O patch só funciona na ISO exatamente igual à usada na tradução. Confira o hash antes de aplicar:

| | Valor |
|---|---|
| Tamanho | 2.913.435.648 bytes |
| MD5 | `565A7D7AC96E3C354D11F32D38A18B41` |
| SHA-1 | `507F98E24A0B4464C717FA05E7DA9EADA3B78708` |

Para ver o hash no Windows, rode no PowerShell:

```
Get-FileHash "Digimon World - Data Squad.iso" -Algorithm MD5
```

No Linux ou macOS, use `md5sum arquivo.iso` ou `md5 arquivo.iso`.

Se o hash não bater, a ISO é de outra versão (europeia, japonesa) ou foi alterada, e o patch vai recusar ou gerar um jogo quebrado.

---

## Como aplicar o patch

### Windows: Delta Patcher (mais fácil)

1. Baixe o **Delta Patcher** no GitHub (*marco-calautti/DeltaPatcher*, em *Releases*).
2. Abra o programa.
3. Em **Original file**, escolha a sua ISO americana.
4. Em **XDelta patch**, escolha o arquivo `.xdelta`.
5. Clique na engrenagem e marque **"Backup original file"** se quiser manter uma cópia da ISO em inglês. Recomendado.
6. Clique em **Apply patch** e espere a mensagem de sucesso.

### Qualquer sistema: xdelta3 na linha de comando

Baixe o `xdelta3` (*jmacd/xdelta-gpl* no GitHub, ou pelo gerenciador de pacotes do Linux/macOS) e rode:

```
xdelta3 -d -s "Digimon World - Data Squad.iso" "Digimon World - Data Squad PT-BR v0.9.xdelta" "Digimon World - Data Squad (PTBR).iso"
```

Assim a ISO original fica intacta e sai um arquivo novo, já traduzido.

### Confira o resultado

A ISO traduzida deve ter:

| | Valor |
|---|---|
| MD5 | `E8FC6360F72BF91C4DAA08133A31CF4F` |
| SHA-1 | `D2502B8D7ACF822FA9F525473A41E9379CFCEB04` |

---

## Configuração recomendada no PCSX2

- **Desligue o patch de widescreen (tela larga) para este jogo.** Com ele ligado, o texto passa da borda da caixa de diálogo. Isso acontece também no jogo original em inglês.
  - Clique com o botão direito no jogo > **Propriedades** > desmarque **Widescreen Patches**.
- O executável do jogo foi alterado (alguns textos da interface ficam nele). Por isso o PCSX2 enxerga o jogo traduzido com outro **CRC** (`742E44A7`), diferente do original (`7E582398`). Configurações por jogo, cheats e patches feitos para o original não passam sozinhos para a versão traduzida: refaça-os no jogo traduzido.
- **Saves:** o save da versão em inglês funciona na traduzida, porque o código do jogo (SLUS-21598) é o mesmo.

A tradução foi testada no PCSX2. Em PS2 de verdade (OPL etc.) ainda não foi testada. O tamanho e a estrutura do disco são os mesmos do original, então deve funcionar; se testar, conte nas *Issues*.

---

## Escolhas de tradução

- Nomes como na versão americana: Marcus, Agumon, Yoshino, Thomas, Kudamon, Sampson, Kagura, DATS, DigiSoul Charge.
- *Rookie / Champion / Ultimate / Mega* viraram **Novato / Campeão / Supremo / Mega**.
- *Tamer* virou **Domador**; *Dark Area*, **Área Sombria**; *DigiEgg*, **DigiOvo**.
- Os Sete Pecados (Seven Sins) foram traduzidos: Preguiça, Ganância, Luxúria, Inveja, Gula, Ira, Orgulho.
- As caixas de texto do jogo cabem 24 letras por linha. As frases foram reescritas para caber sem cortar.

---

## Créditos

- **Tradução, revisão e testes:** renanfusion6
- **Ferramentas e romhacking:** renanfusion6

## Aviso legal

Projeto de fã, sem fins lucrativos e sem ligação com a Bandai Namco ou a Toei Animation. *Digimon* e *Digimon World Data Squad* pertencem aos seus donos. Este repositório distribui **apenas o patch de tradução**. Para jogar, use uma cópia do jogo que você tenha. Não peça nem compartilhe ISOs aqui.
