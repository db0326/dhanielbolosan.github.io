---
layout: project
type: project
image: img/rock-paper-scissors/rock-paper-scissors-icon.png
title: "Rock Paper Scissors"
date: 2023
published: true
labels:
  - Java
  - Swing
  - User Interface
summary: "My first user interface"
---
## Rock, Paper, Scissors... Swing?
My first experience with scripting a user interface involved developing a simple Rock-Paper-Scissors game using Java and Swing. In this program, the user plays a game of Rock-Paper-Scissors against the computer and features a straightforward interface with buttons for Start, Instructions, Exit, and the three game choices—Rock, Paper, and Scissors. Additionally, the user interface has a display area showing game results and messages.

## Code Leak-oko
The project was divided into three ```.java``` files: 
<ul>
  <li>```Game.java`` which handled the game mechanics</li>
  <li>```GUIFrame.java``` which created the user interface and managed events</li>
  <li>```RPS.java``` which served as the driver</li>
</ul>
The game logic uses numerical values to represent game choices: 0 for Rock, 1 for Paper, and 2 for Scissors. A random number generator was then used to generate the computer’s choice based on these values, which is then compared with the player’s choice to determine the outcome of each round. 

```
 public void playRound(int userChoice) {

        // Make the random number become the computer's choice
        computerChoice = randomNumber();

        // Convert the random number to "Rock", "Paper", or "Scissors"
        String computerChoiceString = choices[computerChoice];

        // Print computer's choice to terminal (this was used in early testing)
        System.out.println("Computer chose: " + computerChoiceString);

        // If both choices are the same, it's a tie
        if (userChoice == computerChoice){
            System.out.println("Tie");          // Print "Tie" in terminal (early testing)
            tieCounter++;                         // Increase Tie Counter
            userWins = false;                     // Change userWins bool to false
        // Else if user beats computer, user wins
        } else if ((userChoice == 0 && computerChoice == 2) ||
                    (userChoice == 1 && computerChoice == 0) ||
                    (userChoice == 2 && computerChoice ==1)) {
            System.out.println("You win!");     // Print "You win!" in terminal (early testing)
            userScore++;                          // Increase User Score
            userWins = true;                      // Change userWins bool to true
        // Else user loses
        } else {
            System.out.println("You lose");     // Print "You lose" in terminal (early testing)
            computerScore++;                      // Increase Computer Score
            userWins = false;                     // Change userWins bool to false
        }

    }
```
