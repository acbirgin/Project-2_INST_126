# Project-2_INST_126
## Step 1 - Implementing the Hangman game
In order to randomize the hangman concept, it was necessary to use the **import statement** - which is the first line of code before the list.
I then defined the function, making it callable at the end in order to actually play the hangman game.
Next, in a sequential order, I set up the code in a way that assigned a variable to a list of random, mixed words in a list. Using different variables, the hangman game gives the user a maximum of 10 incorrect guesses with the option for repeatable letters (and not being penalized for repeating letters).
The first loop is meant to call on an empty list, assigned by the variable *temp.* There, it recognizes the list position that was randomized, and adds it to the end of the index position.
The second loop is meant to utilize user input given a letter. Here, it is important that the program doesn't give a false error when the user guesses a correct letter, but uses a lowercase format. This is solved by using the .upper method, which makes the guess correct uppercase letter (corresponding to the uppercase letters in the list values). The program then removes a correctly guesses letter from the index position using the .pop method, so there isn't any unnecessary repetition.
Print statements are then used depending on whether or not the letter is guessed correctly.

## Step 2 - Implementing the encrypt() function
Using the **plaintext** argument, I started off by setting variable **ciphertext** equal to an empty string value. 
Using a **for** loop, I then set it up to where ciphertext would return an index value depending on whether the index value was odd or even.
by setting the **plain_ascii** variable equal to the index value of the **plaintext** index position.
The variable cipher_ascii takes the index value of the empty string value of **ciphertext** and adds it to the index position (opposite for odd index values)
Lastly, I return the value of **ciphertext** equaling the index position of the guessed letter.

## Step 3 - Making the decrypt() function
In order to reverse the order of the encrypt function, decrypt takes **ciphertext** as the argument in the function and returns the **plaintext** value.
Here, I used the same steps in the encrypt() function, but in reverse order. Essentially, if even, the index value is subtracted and the odd index value is subtracted.

## Step 4 - Calling All of the Functions
In the final cell, **ranWord** variable along with the encryption of **ranWord** and decryption of the same variable, are called.
