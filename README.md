# 🧩 8-Puzzle Interativo: O Jogo que Fala Contigo!

[![C Language](https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white)](https://en.wikipedia.org/wiki/C_(programming_language))
[![CLI Game](https://img.shields.io/badge/Interface-CLI%20(Terminal)-8E44AD?style=for-the-badge)](#)
[![License](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](LICENSE)

> Uma implementação clássica do jogo **8-Puzzle** (Deslizar peças) desenvolvida em **C** puro[cite: 12]. O grande diferencial deste projeto é o seu **sistema de progressão narrativa**: à medida que perdes tempo e acumulas dezenas de movimentos, o próprio jogo começa a ganhar consciência, conversando contigo, oferecendo a desistência e até narrando a sua própria vida!

---

## 🎯 Sobre o Projeto

O 8-Puzzle é um quebra-cabeças deslizante que consiste num tabuleiro 3x3 com 8 blocos numerados e um espaço vazio[cite: 12]. O objetivo é ordenar os números de 1 a 8, deixando o vazio no final[cite: 12].

Este projeto foi construído para praticar manipulação de matrizes, ponteiros (para rastrear a posição do espaço vazio) e leitura direta de teclado (`getch()`) em C[cite: 12]. Para garantir que o jogo seja sempre resolúvel, o tabuleiro não é embaralhado aleatoriamente do zero; em vez disso, ele parte do estado final e executa 25 movimentos aleatórios válidos no início[cite: 12].

### 🌟 Destaques do Projeto
- 🎮 **Controles WSAD:** Interface fluida onde não precisas de premir *Enter* após cada movimento, graças à função `getch()`[cite: 12].
- 🧠 **Sistema "Anti-Stress" (ou Pró-Stress):** A cada 20 movimentos, o jogo interrompe a partida com mensagens de texto únicas e hilariantes, questionando a tua resiliência e oferecendo-te uma saída honrosa[cite: 12].
- 🛡️ **Embaralhamento Seguro:** Previne o "Problema da Paridade" do 8-puzzle (onde 50% dos tabuleiros gerados aleatoriamente são impossíveis de resolver) simulando movimentos reais para gerar o estado inicial[cite: 12].
- 📐 **Renderização Limpa:** A função `system("cls")` garante que o tabuleiro se atualiza na mesma posição do terminal, criando uma ilusão de interface estática[cite: 12].

---

## 🕹️ Como Jogar

1. **O Tabuleiro:** O espaço vazio é representado pelo caractere `|⌂ |` (ou similar, dependendo do teu terminal)[cite: 12].
2. **Movimentação:** Usa as teclas clássicas de movimento (o espaço vazio é o que se move):
   - `W` (Cima)
   - `S` (Baixo)
   - `A` (Esquerda)
   - `D` (Direita)
3. **O Objetivo:** Organiza a matriz para que fique exatamente nesta ordem:
   ```text
   |1| |2| |3|
   |4| |5| |6|
   |7| |8| |⌂|

```

4. **Interrupções:** A cada 20 movimentos, o jogo fará uma pausa. Responde com `1` (Sim, quero desistir) ou `0` (Não, vou continuar).



---

## 🎭 A Narrativa Oculta

Se fores teimoso o suficiente para chegar aos 180 movimentos, prepara-te para a despedida emocional do teu puzzle, que te deixará nas mãos do seu filho: o "8-puzzle Jr".

---

## 🛠️ Tecnologias e Bibliotecas

* **Linguagem:** C (Padrão ANSI)
* **Bibliotecas Standard:**
* `<stdio.h>`: I/O (printf, scanf).


* `<stdlib.h>`: Geração de *seeds* (`srand`, `rand`), e função `exit()`.


* `<time.h>`: Utilizada para alimentar o `srand()` com o tempo real do sistema, garantindo embaralhamentos diferentes a cada execução.


* `<conio.h>`: Fornece a função `getch()` para captura instantânea de teclas sem a necessidade de buffer do teclado (Windows).





---

## 📂 Estrutura do Repositório

```text
8-Puzzle-Game/
├── projeto_8_puzzle.c       # Código fonte completo do jogo
├── projeto_8_puzzle.exe     # Executável compilado (Windows)
└── README.md                # Documentação do projeto

```

---

## 🚀 Como Executar o Projeto

### 📋 Pré-requisitos

Precisas de um compilador de C instalado na tua máquina (ex: GCC/MinGW) e um ambiente Windows (devido à dependência da biblioteca `<conio.h>` e do comando `cls`).

### 1. Compilação via Terminal

Abre o terminal na pasta do ficheiro e executa:

```bash
gcc projeto_8_puzzle.c -o puzzle

```

### 2. Executar o Jogo

Inicia o executável criado:

```bash
puzzle.exe

```

---

## 👥 Equipe de Desenvolvimento

Este projeto foi desenvolvido em grupo no âmbito do curso de **Ciência de Dados e Inteligência Artificial** na PUC-Campinas.

* **Henrique Royale** - [GitHub](https://github.com/HenriqueRoyale?utm_source=gemini)
* **Lucas Rosário Gomes** - [Ainda não possui Github]
* **Gabriel Monteiro Zavatta** - [Ainda não possui Github]
* **Igor Heizo Miyashita** - [Ainda não possui Github]

---

*Desenvolvido com ☕, trabalho de equipa, ponteiros e uma pitada de crise existencial computacional.*

```

```
