# Hangman-Game
The provided Ruby code is an implementation of the classic word-guessing game, Hangman. It allows the user to guess letters to reveal a hidden word. Below is a breakdown of the code:

1. The `Hangman` class is defined, and its constructor (`initialize`) initializes the game's state. It selects a random word from the `words` array, sets the number of lives to 7, and creates a word teaser (with underscores for each letter in the word).

2. The `words` method is an array of word-clue pairs. These are the words that the player will guess, along with a clue for each word.

3. The `print_teaser` method is used to display the current state of the word teaser. It takes an optional argument `last_guess` to update the teaser after each guess.

4. The `update_teaser` method updates the word teaser based on the user's guess. It replaces underscores in the teaser with the guessed letter if it's correct.

5. The `make_guess` method handles the player's guess. It prompts the user to enter a letter, checks if it's correct, updates the teaser, and handles game over or a win conditions.

6. The `begin` method starts the game, displays the initial teaser, and provides a clue. It then calls `make_guess` to start the game.

7. An instance of the `Hangman` class is created, and the game is started by calling the `begin` method.

To play the game, run the Ruby script. The user guesses letters one by one until they either complete the word or run out of lives.

You can customize the word list, the number of lives, and other aspects of the game by modifying the `initialize` method and the `words` array in the `Hangman` class.
