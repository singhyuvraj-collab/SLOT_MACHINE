SLOT MACHINE
A simple command-line based Slot Machine game developed in Python.

  # Features
- Player name input
- Minimum deposit requirement
- Maximum deposit limit
- Random slot symbols
- Different values for each symbol
- Matching symbol rewards
- Jackpot system
- Balance tracking
- Total winnings tracking
- Final game summary

  

   # Technology used
- Python 3
- Random module

  # WORKFLOW OF THE PROGRAM : 

The program follows this general flow:
Start
  >
Enter Player Name
  >
Enter Starting Money
  >
Check Starting Money
  >
Generate 3 Random Symbols
  >
Check Symbol Combination
  >
Calculate Reward
  >
Update Balance
  >
Ask Whether to Continue
  >
Continue / Stop
  >
Display Game Summary
  >
End

## 🎰 How It Works

The Slot Machine is a simple Python-based game where the player deposits an amount of money and spins the slot machine to try to win rewards.

### 1. Player Setup

* The player enters their name.
* The player enters the amount of money they want to deposit.
* The minimum balance required to play is **20**.
* The maximum allowed deposit is **1000**.
* If the deposited amount is below 20 or above 1000, the game ends.

### 2. Slot Machine Symbols

The game uses five different symbols:

* `7` → 100 points
* `🍊` → 10 points
* `⭐` → 20 points
* `❤️` → 30 points
* `🏆` → 50 points

Three symbols are randomly selected for every spin using Python's `random` module.

### 3. Spin System

Each spin costs **20** from the player's balance.

The player can make a maximum of **5 spins**, provided they have enough money to continue.

The game keeps track of:

* Total number of spins
* Total winnings
* Starting money
* Current/final money

### 4. Winning Conditions

After three symbols are generated, the game checks different combinations:

* **Three `7`s** → Jackpot reward of **500**
* **Three identical symbols** → Product of their individual values
* **First and third symbols match** → Sum of their values
* **Second and third symbols match** → Sum of their values
* **First and second symbols match** → Sum of their values
* **No matching symbols** → No reward

### 5. Balance Update

If the player wins a reward, the **20 spin fee is refunded** along with the reward.

If the player loses, the **20 spin fee is deducted** from their balance.

The total winnings are also updated after every successful spin.

### 6. Continue or Stop

After each spin, the player is asked whether they want to spin again.

The game stops when:

* The player chooses **"no"**
* The player's balance falls below **20**
* The player reaches the maximum of **5 spins**

### 7. Game Summary

At the end of the game, a summary is displayed containing:

* Player's name
* Starting money
* Total number of spins
* Total winnings
* Final remaining money

This allows the player to see their complete game result after finishing.


# image of the output in VS CODE
<img width="1470" height="502" alt="image" src="https://github.com/user-attachments/assets/bbcd1356-f018-4481-a66a-21f39ecacc30" />
