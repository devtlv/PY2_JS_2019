### Countdown Game

#####  For this project you have to think by yourself of :
##### * the functionnalities
##### * the database and tables
##### * the routes
##### * the templates

The popular British TV game-show, **[Countdown](https://www.youtube.com/watch?v=lsFAokXCxTI)**, asks players to guess as many words as they can from a group of random letters. Whichever player can find the longest word out of all of those letters, wins the game. We will create our own version of this for the Python console.
1.	Pick a long word at random from the database – 9 letters or longer. ([This](https://www.postgresql.org/docs/current/functions-string.html) might help you)
You can use the database you created for *Week9/Day1 Exercise 1*
2.	Mix up the letters of the word at random.
3.	Display it to the user, and start a timer.
4.	Until the time is up (30 seconds by default, but make this adjustable somewhere in your code), prompt the user to type in words. Also tell the user how much time is left. (Use the time module’s perf_counter function. See [here](https://www.programcreek.com/python/example/82530/time.perf_counter) for some code examples (not all of them are very good))
5.	When the time is up, print a message saying that the time is up. If the time is up while the program is waiting for user input, don’t include their last input. Instead, print a message saying something like this: “Sorry, time is up. This guess will not be counted.”
6.	Once time is up, examine the user’s guesses, and award him points as follows:
1.	For a valid word 2 letters long– 1 point.
2.	For a valid word 3 letters long – 3 points
3.	For a valid word 4 letters long – 4 points, etc.
7.	If the player guesses the entire word, print them a message of warm congratulations! :)
8.	Display the player’s final score, and ask for their name. Add them onto a high score board, which will display the top 10 players and their scores.
9.	Offer the player to play again.
10.	If the player decides to play again, make sure that you don’t re-use any words from an earlier game.
