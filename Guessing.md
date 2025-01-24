```mermaid
flowchart TD
1([Start]) --> 2[Generate Random Number]
2 --> 3[Initialize Attempt Counter to 0]
3 --> 4[Prompt User for Guess]
4 --> 5{Is Input Numeric?}
5 --> No --> F[Display "Invalid Input" Message]
6 --> 4
7 --> Yes --> G{Is Guess within Range?}
8 --> No --> H[Display "Out of Range" Message]
9 --> 4
10--> Yes --> I[Compare Guess to Random Number]
11--> Correct Guess --> J[Display "Correct Guess" Message]
12--> K[Ask if User Wants to Play Again]
13--> L{Play Again?}
14--> Yes --> 1
15--> No --> M[End Game]
16--> Guess Too High --> N[Display "Too High" Message]
17--> 4
18 -- Guess Too Low --> O[Display "Too Low" Message]
19 --> 4

1. Start Game:
 The game begans when a randome number is generated and the attempt counter is set to zero.
2. Generate Random Number:
 The system will generate a random number within a certain range, for example, 1 to 100. The number that is generated is what the player must guess.
3. Start Attempt Counter:
 A counter for the number of attempts is started, this will track how many times the player guesses
4. Prompt User for Guess
 The user is prompted to input a guess.
5. Is Input Numeric?:
 The game checks if the user's input is a valid number
 If the input is not a number, an error message will pop up and the user will be prompted to enter a valid guess
 If the input is a number, the game will proceed to check if the guess is correct
6. Is guess within Range?:
 The game checks whether the guess is within the range
 If the game is out of the range, an error message will pop up and tell the user to input a guess thats within the range
 If the guess is within the range, the game continues to check if it the correct number
7. Compare Guess to Random Number
 The system compares the guess with the randomly generated number
 If it is correct, the game proceeds to step 8
 If the guess is too high, a message will pop up saying, "Too High" and will ask the user to guess again.
 If the guess is too low, a "Too Low" message will pop up saying, "Too low", and the user is asked to guess again
8. Correct Guess:
 When the player guesses correctly, a "Correct Guess" message is displayed and the player is asked if they want to play again.
9. Ask if the user wants to play again:
 If the player chooses Yes to the play again prompt the game restars from the beginning (step 1)
 If the player chooses No, the game ends
10. End Game:
 The game ends if the user opts not to play again. All resources are cleaned up, and the program terminates.
 
 
