# 🎰 Slot Machine — Python Console Game

A simple **console-based slot machine game built with Python**. The project demonstrates basic Python programming concepts such as variables, lists, dictionaries, conditional statements, loops, functions, user input, and random selection.

## 📌 Features

* Accepts the player's name.
* Allows the player to enter an initial deposit.
* Validates the deposit amount.
* Provides a maximum of **5 spins** per game.
* Charges **20 units** for each spin.
* Randomly generates three slot-machine symbols.
* Calculates rewards based on matching symbols.
* Includes a special **jackpot reward of 500** for three `7`s.
* Tracks total spins and total winnings.
* Displays a final game summary.

## 🛠️ Technologies Used

* **Python 3**
* **random** — Python standard library module

No external Python packages are required.

---

## 📂 Project Structure

```text
Slot-Machine/
│
├── slot_machine.py
└── README.md
```

* `slot_machine.py` — Contains the complete game implementation.
* `README.md` — Project documentation and setup instructions.

---

## ⚙️ Requirements

Before running the project, make sure you have:

* Python 3 installed on your computer.
* A terminal/command prompt.
* The project files downloaded or cloned to your computer.

You can check whether Python is installed by running:

```bash
python --version
```

If that does not work, try:

```bash
python3 --version
```

The project does not require `pip` or any external package installation.

---

## 🚀 Setup and Installation

### Step 1: Clone the Repository

Clone the repository using Git:

```bash
git clone <YOUR-GITHUB-REPOSITORY-URL>
```

Then move into the project directory:

```bash
cd Slot-Machine
```

If you downloaded the repository as a ZIP file instead, extract it and open a terminal inside the extracted project folder.

### Step 2: Verify Python Installation

Run:

```bash
python --version
```

You should see a Python 3 version.

If your system uses `python3`, run:

```bash
python3 --version
```

### Step 3: Install Dependencies

No external dependencies are required.

The project uses Python's built-in `random` module, so there is nothing to install.

### Step 4: Run the Project

Run the following command:

```bash
python slot_machine.py
```

On systems where Python is accessed using `python3`, use:

```bash
python3 slot_machine.py
```

---

## 🎮 How to Play

### 1. Enter Your Name

When the program starts, enter your name.

```text
Enter your name: Yuvraj
```

### 2. Enter Your Deposit

Enter the amount of money you want to use for the game.

```text
enter the amount of money you want to deposit: 100
```

The deposit must satisfy:

* Minimum deposit: **20**
* Maximum deposit: **1000**

If the amount is below 20, the game stops.

If the amount is above 1000, the game stops.

### 3. Spin the Machine

The program randomly selects three symbols.

Example:

```text
⭐ 🍊 ⭐
```

The program checks the symbols and calculates the reward according to the game's rules.

### 4. Continue or Stop

After each spin, the program asks:

```text
Do you want to spin again? yes or no:
```

Enter:

```text
yes
```

to continue or:

```text
no
```

to stop.

The game also stops automatically when:

* The balance becomes less than 20, or
* The player completes 5 spins.

---

## 🏆 Reward System

The game uses the following symbol values:

| Symbol | Value |
| ------ | ----: |
| 🍊     |    10 |
| ⭐      |    20 |
| ❤️     |    30 |
| 🏆     |    50 |
| 7      |   100 |

### Jackpot

If all three symbols are `7`:

```text
7 7 7
```

the player receives a fixed reward of:

```text
500
```

### Three Matching Symbols

If all three symbols are the same, the reward is calculated by multiplying their values.

For example:

```text
⭐ ⭐ ⭐
```

Since ⭐ has a value of 20:

```text
20 × 20 × 20 = 8000
```

### Two Matching Symbols

If two symbols match, their values are added together.

For example:

```text
🍊 ⭐ 🍊
```

The matching symbols are 🍊 and 🍊:

```text
10 + 10 = 20
```

### No Matching Symbols

If none of the symbols match, the reward is:

```text
0
```

The spin cost is not refunded.

---

## 💰 Game Balance

Each spin costs **20 units**.

The program keeps track of:

* Starting money
* Current money
* Number of spins
* Total winnings
* Final money

At the end of the game, a summary is displayed.

Example:

```text
GAME SUMMARY
Thank you for playing: Yuvraj
Your starting money was: 100
Total spins are: 5
Your total winning is: 120
the final money is: 140
```

---

## 🧠 Concepts Demonstrated

This project demonstrates several fundamental Python concepts:

### Variables

Used to store information such as the player's name, balance, number of spins, and winnings.

### Lists

The available slot symbols are stored in a list:

```python
symbols = ["7", "🍊", "⭐", "❤️", "🏆"]
```

### Dictionaries

A dictionary is used to associate each symbol with its value:

```python
symbol_values = {
    "🍊": 10,
    "⭐": 20,
    "❤️": 30,
    "🏆": 50,
    "7": 100
}
```

### Conditional Statements

`if`, `elif`, and `else` statements determine the reward for each combination.

### Loops

A `while` loop allows the player to perform multiple spins while the game conditions are satisfied.

### Functions

The `game_summary()` function displays the final results.

### Random Selection

The `random.choice()` function is used to randomly select the three symbols.

---

## ⚠️ Limitations

This project is a simple educational console application and has some limitations:

* It accepts integer deposits only.
* It does not use a graphical user interface.
* Game results are not saved after the program closes.
* User input validation is limited.
* The game uses Python's standard pseudo-random `random` module.
* The maximum number of spins is fixed at 5.

---

## 🔮 Future Improvements

Possible improvements include:

1. Adding a graphical user interface.
2. Adding better input validation.
3. Creating separate functions for spinning, reward calculation, and balance management.
4. Adding sound and visual effects.
5. Adding persistent player statistics.
6. Adding automated tests for the reward system.
7. Allowing configurable spin limits and game settings.

---

## ▶️ Quick Start

If Python is already installed, the project can be started with:

```bash
git clone <>
cd Slot-Machine
python slot_machine.py
```

No additional packages are required.

---

## 📄 License

This project was created as an educational mini-project for learning and demonstrating fundamental Python programming concepts.


# image of the output in VS CODE
<img width="1470" height="502" alt="image" src="https://github.com/user-attachments/assets/bbcd1356-f018-4481-a66a-21f39ecacc30" />
