# Rock, Paper, Scissors Game

## Overview
This program implements a Rock, Paper, Scissors game where the computer
attempts to predict the user\'s next move based on their past choices.

**Game Rules:**

- **Rock** beats **Scissors**.

- **Scissors** beats **Paper**.

- **Paper** beats **Rock**.

**How to Play:**

1.  The program will prompt you to enter a number representing your
    choice:

    - 0 for Rock

    - 1 for Paper

    - 2 for Scissors

2.  The computer will make its choice based on a prediction algorithm
    that analyzes your previous moves.

3.  The program will display the results of the round and update the
    scores.

4.  The game continues until either you or the computer reaches a score
    of 10.

**Functions:**

- **update_counts(user_input):**

  - This function keeps track of how many times the user has chosen each
    option (rock, paper, scissors).

  - It takes the user\'s input as an argument and increments the
    corresponding counter.

- **predict():**

  - This function predicts the computer\'s next move.

  - It analyzes the counts of user choices and chooses the most frequent
    one.

  - If there is no clear pattern, it chooses randomly.

  - It returns the computers predicted move.

- **update_scores(user_input):**

  - This function determines the winner of each round and updates the
    scores.

  - It takes the user\'s input as an argument and compares it to the
    computer\'s prediction.

  - It prints the result of the round and the current scores.

**Variables:**

- **count_rock, count_paper, count_scissors:** These variables store the
  number of times the user has chosen each option.

- **player_score, comp_score:** These variables store the player\'s and
  computer\'s scores, respectively.

- **valid_entries:** A list containing the valid input values (\'0\',
  \'1\', \'2\').

**Game Logic:**

1.  The game starts with the scores and choice counts initialized to 0.

2.  The program enters a while loop that continues until a player
    reaches a score of 10.

3.  Inside the loop, the program prompts the user for input and
    validates it.

4.  The update_scores() and update_counts() functions are called to
    update the game state.

5.  The loop continues until a winner is determined.

6.  The winner is announced, and the game ends.
