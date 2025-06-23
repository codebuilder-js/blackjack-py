# Blackjack - Python Console Game 🃏

Este é um simples jogo de **Blackjack** (21) que roda no console.
Você joga contra o dealer e tenta chegar o mais próximo possível de 21 sem estourar.

## 🎮 Regras do Jogo

* **Objetivo**: Tente chegar o mais próximo possível de 21 pontos, sem ultrapassar.
* **Valores das Cartas**:

  * Números (2 a 10): Valor da própria carta.
  * J, Q, K: 10 pontos.
  * Ás (A): 1 ou 11 pontos (automático, o que for mais vantajoso).
* **Ações do Jogador**:

  * **(H)it**: Comprar mais uma carta.
  * **(S)tand**: Parar de comprar cartas.
  * **(D)ouble down**: Dobrar a aposta e comprar mais uma carta (somente na primeira jogada).
* **Dealer**:

  * Para de comprar cartas quando atinge 17 ou mais pontos.
* **Empate**: A aposta é devolvida.
* **Vitória**: Você ganha o valor da aposta.
* **Derrota**: Você perde o valor da aposta.

## 💻 Como Jogar

1. Execute o script `blackjack.py`:

   ```bash
   python blackjack.py
   ```

2. Você começa com \$5000.

3. Escolha o valor da aposta em cada rodada.

4. Use os comandos no console para jogar:

   * `H`: Comprar uma carta.
   * `S`: Parar de comprar.
   * `D`: Dobrar a aposta (opcional).

5. O jogo termina quando seu saldo chega a \$0 ou você decide sair com `QUIT`.

## 🧩 Estrutura do Código

* `main()`: Loop principal do jogo.
* `getBet(maxBet)`: Pede o valor da aposta.
* `getDeck()`: Cria e embaralha o baralho.
* `displayHands(playerHand, dealerHand, showDealerHand)`: Exibe as cartas.
* `getHandValue(cards)`: Calcula o valor das mãos.
* `displayCards(cards)`: Imprime as cartas no console.
* `getMove(playerHand, money)`: Lê a jogada do jogador.

## 🚀 Como Rodar o Código

1. Tenha o Python 3.x instalado.
2. Salve o código em um arquivo chamado `blackjack.py`.
3. Execute o comando:

   ```bash
   python blackjack.py
   ```

## 📋 Exemplo de Execução

```
Rules:
Try to get as close to 21 without going over.
...

Money: 5000
How much do you bet? 1 - 5000, or QUIT
> 100

DEALER: ???
PLAYER: 15
(H)it, (S)tand, (D)ouble down> H

You drew a 5 of ♠

PLAYER: 20
(H)it, (S)tand> S

DEALER hits...
...

You won $100!
```
