<div align="center">

# 🎯 Java Sudoku

<img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" />
<img src="https://img.shields.io/badge/IntelliJ_IDEA-000000?style=for-the-badge&logo=intellij-idea&logoColor=white" />
<img src="https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow?style=for-the-badge" />
<img src="https://img.shields.io/badge/Licença-MIT-green?style=for-the-badge" />

<br/>

> *Um jogo de Sudoku desenvolvido em Java — com versão para terminal e interface gráfica.*

</div>

---

## 📋 Sobre o Projeto

O **Java Sudoku** é um projeto desenvolvido em Java que implementa o clássico jogo de lógica **Sudoku**. O objetivo é preencher uma grade 9×9 com números de 1 a 9, garantindo que cada número apareça apenas uma vez em cada linha, coluna e bloco 3×3.

O projeto possui **duas versões**:

| Versão | Branch | Descrição |
|---|---|---|
| 💻 Terminal | `main` | Versão textual, jogada direto no console |
| 🖼️ Interface Gráfica | `ui` | Versão visual com componentes Swing/AWT |

##  Preview (UIMain)
 
  <img src="assets/sudoku-ui.png" alt="Interface Gráfica do Java Sudoku" width="500"/>
 
---

## ✨ Funcionalidades

- ♟️ Tabuleiro de Sudoku 9×9 totalmente funcional
- ✅ Validação automática das jogadas (linhas, colunas e blocos)
- 🎮 Interação via terminal (branch `main`)
- 🖼️ Interface gráfica amigável (branch `interface-grafica`)
- 📐 Estrutura organizada em pacotes Java (`br.com.game`)

---

## 🗂️ Estrutura do Projeto
 
### 💻 Branch `main` — Versão Terminal
 
```
sudoku/
│
├── src/br/com/game/
│   ├── model/
│   │   ├── Board.java            # Lógica do tabuleiro
│   │   ├── GameStatusEnum.java   # Estados do jogo
│   │   └── Space.java            # Representação de cada célula
│   │
│   └── util/
│       ├── BoardTemplate.java    # Templates de tabuleiros pré-definidos
│       └── Main.java             # Ponto de entrada (terminal)
│
├── .gitignore
└── sudoku.iml
```
 
### 🖼️ Branch `ui` — Versão com Interface Gráfica
 
```
sudoku/
│
├── src/br/com/game/
│   ├── model/
|   |   ├── Board.java            # Lógica do tabuleiro
│   │   ├── GameStatusEnum.java   # Estados do jogo
│   │   └── Space.java            # Representação de cada célula
│   │
│   ├── service/
│   │   ├── BoardService.java     # Regras e lógica do jogo
│   │   ├── EventEnum.java        # Eventos da aplicação
│   │   ├── EventListener.java    # Escuta de eventos
│   │   └── NotifierService.java  # Notificações entre componentes
│   │
│   ├── ui/custom/
│   │   ├── button/
│   │   │   ├── CheckGameStatusButton.java  # Botão de verificar status
│   │   │   ├── FinishGameButton.java       # Botão de finalizar jogo
│   │   │   └── ResetButton.java            # Botão de reiniciar
│   │   ├── frame/
│   │   │   └── MainFrame.java              # Janela principal
│   │   ├── input/
│   │   │   ├── NumberText.java             # Campo de entrada numérica
│   │   │   └── NumberTextLimit.java        # Campo com limite de caracteres
│   │   ├── panel/
│   │   │   ├── MainPanel.java              # Painel principal
│   │   │   └── SudokuSector.java           # Setor 3×3 do tabuleiro
│   │   └── screen/
│   │       └── MainScreen.java             # Tela principal do jogo
│   │
│   └── util/
│       ├── BoardTemplate.java    # Templates de tabuleiros pré-definidos
│       ├── Main.java             # Ponto de entrada
│       └── UIMain.java           # Inicialização da interface gráfica 
│
├── .gitignore
└── sudoku.iml
```
 
---
 
## 🌿 Branches
 
```
main                → Versão console (terminal)
interface-grafica   → Versão com interface gráfica (Swing/AWT)
```
 
Para alternar entre as versões:
 
```bash
# Versão terminal
git checkout main
 
# Versão com interface gráfica
git checkout interface-grafica
```
 
---
 
## 🚀 Como Rodar
 
### Pré-requisitos
 
- [Java JDK 11+](https://www.oracle.com/java/technologies/javase-downloads.html)
- [IntelliJ IDEA](https://www.jetbrains.com/idea/) *(recomendado)* ou qualquer IDE Java
### Passo a passo
 
```bash
# 1. Clone o repositório
git clone https://github.com/CamillypSouza/Java-Sudoku.git
 
# 2. Entre na pasta do projeto
cd Java-Sudoku
 
# 3. Escolha a branch desejada
git checkout main              # versão terminal
git checkout interface-grafica # versão gráfica
 
# 4. Compile o projeto
javac src/br/com/game/Main.java
 
# 5. Execute
java -cp src br.com.game.Main
```
 
>  **Dica:** Se estiver usando o IntelliJ IDEA, basta abrir o projeto e clicar em **Run** — ele cuida de tudo automaticamente!
 
---
 
## 🧠 Como Jogar
 
O **Sudoku** segue três regras simples:
 
1. Cada **linha** deve conter os números de 1 a 9, sem repetição.
2. Cada **coluna** deve conter os números de 1 a 9, sem repetição.
3. Cada **bloco 3×3** deve conter os números de 1 a 9, sem repetição.
 
## 🛠️ Tecnologias Utilizadas
 
- **Java** — Linguagem principal
- **Swing / AWT** — Interface gráfica *(branch `interface-grafica`)*
- **IntelliJ IDEA** — IDE de desenvolvimento
- **Git & GitHub** — Controle de versão
