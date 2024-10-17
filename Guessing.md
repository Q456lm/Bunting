```mermaid
flowchart TD
Start(Begin)-->Generate[Generate at random number]
Generate --> Guess[/Ask user what number is /]
Guess --> Decision{Number Picked}
Decision --> |Picks Correct Number| Correct[Gets message that number is correct]
Decision --> |Picks Incorrect Number| Incorrect[Got message that number is wrong]
Incorrect --> Again[Told to pick another number]
Decision --> |Enters invalid value| Invalid[Got message that incorrect value was entered]
Invalid -->Again
Again --> Decision
Correct --> Finish(End)
```
At first the computer generates a random number from 1 to 10 and the user is given a prompt that says something like "Guess a number between 1 and 10." The user is then told if they are right or not and if they are right the program ends. If they are wrong they are asked to enter another number and are told if that is correct or wrong. If they enter something invalid they are told so and asked to restart.