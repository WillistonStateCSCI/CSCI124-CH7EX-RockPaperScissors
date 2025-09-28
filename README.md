# **Programming Example:**  The Game of Rock, Paper, and Scissors
Children often play the game of rock, paper, and scissors. This game has two players,
each of whom chooses one of the three objects: rock, paper, or scissors. If player 1
chooses rock and player 2 chooses paper, player 2 wins the game because paper
covers the rock. The game is played according to the following rules:

- If both players choose the same object, this play is a tie.
- If one player chooses rock and the other chooses scissors, the player
choosing the rock wins this play because the rock breaks the scissors.
- If one player chooses rock and the other chooses paper, the player
choosing the paper wins this play because the paper covers the rock.
- If one player chooses scissors and the other chooses paper, the player
choosing the scissors wins this play because the scissors cut the paper.

Write an interactive program that allows two people to play this game.

**Input** This program has two types of input:
- The users’ responses when asked to play the game.
- The players’ choices.

**Output** The players’ choices and the winner of each play. After the game is over,
the total number of plays and the number of times that each player won
should be output as well.
## Problem Analysis and Algorithm Design
Two players play this game. Players enter their choices via the keyboard. Each
player enters **R** or **r** for Rock, **P** or **p** for Paper, or **S** or **s** for Scissors. While the
first player enters a choice, the second player looks elsewhere. Once both entries
are in, if the entries are valid, the program outputs the players’ choices and declares
the winner of the play. The game continues until one of the players decides to quit
the game. After the game ends, the program outputs the total number of plays and
the number of times that each player won. This discussion translates into the
following algorithm:
1. Provide a brief explanation of the game and how it is played.
2. Ask the users if they want to play the game.
3. Get plays for both players.
4. If the plays are valid, output the plays and the winner.
5. Update the total game count and winner count.

This program is divided into the following functions, which the ensuing sections
describe in detail.
- **displayRules:** This function displays some brief information about the
game and its rules.
- **validSelection:** This function checks whether a player’s selection is valid.
The only valid selections are R, r, P, p, S, and s.
- **retrievePlay:** Because enumeration types cannot be read directly, this function converts the entered choice (R, r, P, p, S, or s) and returns the
appropriate object type.
- **gameResult:** This function outputs the players’ choices and the winner of
the game.
- **convertEnum:** This function is called by the function gameResult to
output the enumeration type values.
- **winningObject:** This function determines and returns the winning
object.
- **displayResults:** After the game is over, this function displays the final
results.

**__Note:  See chapter 7 of from C++ Programming: From Problem Analysis to Program Design by D.S. Malik for more detailed information on this example.__**

7. Repeat Steps 2 through 5 while the users agree to play the game.
8. Output the number of plays and times that each player won.
We will use the enumeration type to describe the objects.
