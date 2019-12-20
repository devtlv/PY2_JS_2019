### Exercise 1: Form and database

We’re all used to Autocomplete when we fill in online forms. You start typing in a text field, and the page shows a list of words that you might want to type, eg. when you start typing on a search engine page (such as Google). We will create our own version of this for the Python console.
1.	Create a new database called word-games.
2. Download the file : https://www.mit.edu/~ecprice/wordlist.10000
3.	Write a script to import the file into your new database.
4.	You will need to create a table for the word list. What fields will it need? What data types?
5.	Use test data while building your script, until you’re sure it will work properly. Then run it with the real word list file.
6.	Now create a new Python project called game_autocomplete
7.	Create a class called Autocomplete. Create a class method named get_autocomplete_list(text), which will connect to the database, fetch a list of the relevant words, and return them as a list..
8.	Create a route and a template with a form. Think about user-friendliness. How many words should you show to the user for autocompleting?
9.	Now for the user interface (UI). Until the user enters an empty string, accept more input. When the user presses <Enter>, display a list of autocompletions for the text that she has typed in.
10.	What if the user types in a whole word? Or more than one word, eg. “hello wor”? What if the user types in a word for which there are no autocompletions? Make sure your program functions sensibly and gracefully in all of these cases.


### Exercise 2: Continuing the autocomplete Exercise
1. Make each word in the list of autocomplete words clickable, so the user can choose the word that he wants

### Bonus : 
1.  Change the text file by this file:  https://raw.githubusercontent.com/sujithps/Dictionary/master/Oxford%20English%20Dictionary.txt 
In order to give the definition of each word to the user when you render the autocomplete list of words. 
How should the table of the database change ?
