# Rock, Paper, Scissors Game

This is a simple implementation of the classic Rock, Paper, Scissors game in Python. The user plays against the computer, which randomly selects one of the three options: rock, paper, or scissors. The game then determines the winner based on the choices made by both the user and the computer.

## Features

- Simple and intuitive gameplay.
- Randomized computer choices for unpredictable gameplay.

## Installation

1. **Clone the repository:**

    ```
    git clone https://github.com/Rafsun07/Rock-Paper-Scissors.git
    cd rock-paper-scissors
    ```

2. **Run the game:**

    ```
    python rock-paper-scissors.py
    ```

## Usage

1. **Start the game:**

    Run the `rock-paper-scissors.py` script to start the game.

    ```
    python rock-paper-scissors.py
    ```

2. **Input Prompts:**

    Enter your choice by typing 'r' for rock, 'p' for paper, or 's' for scissors.
    
4. **Output:**
    - The computer will randomly select its choice.
    - The result of the game will be displayed, indicating whether you won, lost, or it's a tie.

## How the Code Works

1. **Importing Libraries:**
   
   ```
   import random
   ```
   
- The code imports the random module from the Python Standard Library. This module is used to generate random choices for the computer player in the game.

2. **Defining the `play()` Function:**

   ```
   def play():
   ```

- This function is the main entry point for playing the Rock Paper Scissors game.

3. **Getting User Input:**

   ```
   user = input("What's your choice? 'r' for rock, 'p' for paper, 's' for scissors\n")
   ```
   
- The code prompts the user to input their choice of 'r' for rock, 'p' for paper, or 's' for scissors.

4. **Generating Computer's Choice:**

   ```
   computer = random.choice(['r', 'p', 's'])
   ```
   
- The code randomly selects one of the options ('r', 'p', or 's') for the computer player using the random.choice() function.

5. **Determining the Winner:**

   ```
   if user == computer:
      return 'It\'s a tie'
   ```
    
- If the user's choice is the same as the computer's choice, the game ends in a tie.

6. **Checking Win Conditions:**

   ```
   if is_win(user, computer):
      return 'You won!'
   ```
    
- If the user's choice beats the computer's choice based on the game rules (rock beats scissors, scissors beats paper, paper beats rock), the user wins.

7. **Checking Lose Conditions:**

   ```
   return 'You lost!'
   ```
   
- If none of the above conditions are met, the user loses the game.

8. **Defining the `is_win()` Function:**

   ```
   def is_win(player, opponent):
   ```
   
- This function determines if the player wins against the opponent based on the game rules.

9. **Winning Conditions:**

   ```
   if (player == 'r' and opponent == 's') or (player == 's' and opponent == 'p') \
       or (player == 'p' and opponent == 'r'):
       return True
   ```
   
- If the player's choice beats the opponent's choice according to the game rules (rock beats scissors, scissors beats paper, paper beats rock), the function returns True.

10. **Printing the Result:**

    ```
    print(play())
    ```
    
- Finally, the code calls the play() function and prints the result of the game.

  
That's a basic breakdown of how the Rock Paper Scissors game code works. It takes user input, generates a random choice for the computer, compares the choices to determine the winner, and prints the result.


## Contributing

Contributions are welcome! Please fork the repository and create a pull request with your changes. Ensure that your code follows the project's coding standards and includes appropriate tests.

## Contact

For questions, suggestions, or issues, please open an issue on GitHub or contact the project maintainer at [rafsun.eram@gmail.com](mailto:rafsun.eram@gmail.com).

## Acknowledgements

- Developed using Python.
- Inspired by Rock, Paper, Scissors.

---
