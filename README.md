# break_substitution_cipher

The given code is a Python script that performs decryption of a substitution cipher. It involves the following components:

It defines a variable BOOK_FILE_NAME that initially stores the name of an encrypted book file. However, in the next line, the variable is reassigned a multi-line string representing the encrypted text itself. The encrypted text represents the content of a book or document.

It defines a function frequency that takes a string (cipher_source) as input and analyzes the frequency of letters in the string. The function performs the following steps:

It initializes an empty dictionary letter_frequency to store the frequency of each letter.
The input string is converted to lowercase and all non-alphabetic characters are removed.
The function loops through each letter in the cleaned-up string and updates the letter_frequency dictionary accordingly.
The letter_frequency dictionary is sorted in descending order by frequency.
A pre-defined dictionary frequency_table is created, which contains the average frequency of letters in the English language.
The frequency_table dictionary is sorted in descending order by frequency.
The sorted letter_frequency dictionary is returned.
It defines a function decrypt that takes a string (cipher_source) as input and performs the decryption of a substitution cipher. The function performs the following steps:

It defines two strings: plain_text_alphabet representing the plaintext alphabet and cipher_text_alphabet representing the corresponding ciphertext alphabet.
It creates a dictionary cipher_to_plain that maps each ciphertext character to its corresponding plaintext character based on the pre-defined substitution alphabet.
The function iterates over each character in the cipher_source string and replaces it with the corresponding plaintext character using the cipher_to_plain dictionary. If the character is uppercase, it converts the corresponding plaintext character to uppercase as well.
The decrypted plaintext is stored in the plain_text variable and returned.
It defines a function main that serves as the entry point of the program. It sets the cipher_source variable to the value of the BOOK_FILE_NAME variable (which contains the encrypted text). Then, it calls the decrypt function with cipher_source as input and prints the decrypted plaintext to the console.

The main function is executed only when the script is run directly (not imported as a module) by checking the __name__ variable. This allows the main function to be executed when the script is run as the main program.

In summary, the code decrypts a substitution cipher by analyzing the frequency of letters in the encrypted text and performing a character-by-character substitution using a pre-defined substitution alphabet. The decrypted plaintext is then printed to the console
