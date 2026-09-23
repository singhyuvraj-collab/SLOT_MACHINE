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

  # Game Rules
- Minimum amount required to spin: 20
- Maximum deposit: 500
- Three `7` symbols give a jackpot reward of 500.
- Three identical symbols give a multiplied reward.
- Two matching symbols give the sum of their values.

   # Technology used
- Python 3
- Random module

The game uses five different symbols:

 SYMBOL -> VALUE 
 7  ->  100
🍊 ->  10  
⭐ ->  20  
❤️ ->  30 
🏆 ->  50 
The values are stored in a Python dictionary and are used when calculating rewards.

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

# Winning Conditions

The program checks the symbols in the following order:

1. *Three 7s*
   - Jackpot reward of 500.
2. *Three identical symbols*
   - The values of the three symbols are multiplied.
3. *First and third symbols match**
   - Their values are added.
4. *Second and third symbols match*
   - Their values are added.
5. *First and second symbols match*
   - Their values are added.
6. *No matching symbols*
   - No reward is given.

# image of the output in VS CODE
<img width="1470" height="502" alt="image" src="https://github.com/user-attachments/assets/bbcd1356-f018-4481-a66a-21f39ecacc30" />

# image of the output in powershell
<img width="1317" height="796" alt="image" src="https://github.com/user-attachments/assets/265b4597-b726-4dc3-acfb-f0fc948e3048" />

