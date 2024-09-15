# Language-translator-
This Python code uses the googletrans library to translate text from one language to another.

Code Walkthrough:
Install the Library:

pip install googletrans==4.0.0-rc1: Installs the googletrans library, specifically version 4.0.0-rc1, which is used for translating text via Google Translate.
Import the Translator:

from googletrans import Translator: Imports the Translator class from the googletrans module, which provides the functionality to translate text.
translate_text Function:

Purpose: This function accepts a piece of text and the destination language code, then returns the translated text.
translator = Translator(): Creates an instance of the Translator class.
translator.translate(text, dest=dest_language): Calls the translate method of the Translator class, passing in the text to translate and the dest_language as the target language (using a language code like "es" for Spanish).
return translated_text.text: The translate method returns an object that contains the translated text, and this line returns just the translated text.
main Function:

Purpose: Handles user input and calls the translate_text function.
input_text = input("Enter text to translate:"): Prompts the user to input the text that they want to translate.
target_language = input("Enter target language"): Prompts the user to input the destination language code (e.g., "ja" for Japanese).
translated_text = translate_text(input_text, target_language): Calls the translate_text function, passing the user’s input text and the target language.
print("Translated text:", translated_text): Prints the translated text.
Entry Point:

if __name__ == "__main__": main(): This ensures that the main() function is only executed if the script is run directly, not imported as a module.
Key Concepts:
Translation: The code takes input text, translates it using Google Translate, and prints the result.
User Input: It requires the user to provide both the text and the destination language.
