🔐 Python Caesar Cipher
A simple command-line Caesar cipher tool built with Python. This program lets users encrypt or decrypt messages by shifting letters of the alphabet by a chosen number. It's a great beginner project for learning about functions, lists, string manipulation, and modular arithmetic in Python.

📖 Python Caesar Cipher
The Python Caesar Cipher is a console-based application that implements the classic Caesar cipher — one of the oldest and simplest encryption techniques. Each letter in the message is shifted forward (to encrypt) or backward (to decrypt) by a specified number of positions in the alphabet.

When the program starts, the user is asked to choose between encrypt (e) and decrypt (d), then enters a message and a shift number. The program then outputs the transformed text. Non-alphabetic characters (spaces, punctuation, numbers) are preserved as-is, and the shift wraps around the alphabet using modulo arithmetic.

After each run, the user can choose to try again with a new message, mode, and shift — making it easy to experiment with different cipher shifts.

✨ Features
Two modes – Encrypt (e) or decrypt (d).

Custom shift amount – Choose any whole number to shift letters by.

Automatic wrapping – Shift values are taken modulo 26 so large numbers work smoothly.

Preserves non-letters – Spaces, punctuation, and digits remain unchanged.

Case-insensitive input – Messages are converted to lowercase for consistent handling.

Input validation – Rejects invalid mode choices and non-numeric shift inputs.

Repeat option – Try again with a new message without restarting the program.

Clean user prompts – Clear guidance at every step.

🛠️ What It Uses
Language & Library
Python 3 – No external libraries required (pure standard library).

Key Variables
Variable	Purpose
alphabet	A list of lowercase letters a–z used for shifting.
mode	Stores whether the user wants to encrypt (e) or decrypt (d).
text	The message to be encrypted or decrypted.
shift	The number of positions to shift each letter.
Key Functions
Function	Purpose
get_valid_mode()	Prompts the user until a valid mode (e or d) is entered.
get_valid_shift()	Prompts the user until a valid whole number is entered, then applies modulo 26.
caesar(start_text, shift_amount, mode)	Performs the encryption/decryption and handles the repeat prompt.
Python Concepts Demonstrated
Functions – Organizing logic into reusable blocks.

Lists – Using a list of letters as the alphabet.

alphabet.index() – Finding a letter's position.

Modular arithmetic – (position + shift) % 26 to wrap around the alphabet.

Loops – while True loops for input validation and for loops for processing text.

Conditional logic – Handling encryption vs. decryption.

Exception handling – try/except blocks for safe shift input.

String methods – .lower() and .strip() for clean input.

Recursion – The caesar() function calls itself when the user chooses to try again.

F-strings – Formatted output for the result message.

Keyword arguments – Calling caesar(start_text=..., shift_amount=..., mode=...).

Built-in Functions Used
input() – Reads user input from the console.

print() – Displays prompts and results.

int() – Converts the shift input into a whole number.

len() – Not used directly but relevant to the alphabet's fixed length (26).

📥 Download
You can download the source file from this repository and save it as a .py file:

text
caesar_cipher.py
No installation or dependencies are needed — just Python.

▶️ How to Run
Make sure you have Python 3 installed (python.org).

Save the code as caesar_cipher.py.

Open a terminal or command prompt in the folder containing the file.

Run:

bash
python caesar_cipher.py
Follow the prompts to encrypt or decrypt your message.

🖥️ Example Session
text
Would you like to encrypt (e) or decrypt (d)? e
Enter your message: 
hello world
Enter the shift number: 
3
Here's the encrypted result: khoor zruog
Would you like to try again? (y/n) y
Would you like to encrypt (e) or decrypt (d)? d
Enter your message: 
khoor zruog
Enter the shift number: 
3
Here's the decrypted result: hello world
Would you like to try again? (y/n) n
Thanks for playing.
🐍 Made with Python
This project is written entirely in Python 3 using only the standard library. It's a clean and practical example of how functions, lists, and modular arithmetic can be combined to implement a classic cipher.

Whether you're a beginner practicing string manipulation or someone interested in basic cryptography, this project is a great starting point.

💡 Possible Future Improvements
Preserve original letter casing – Keep uppercase letters uppercase in the output.

Support negative shifts directly in the prompt.

Brute-force mode – Try all 26 shifts to crack an unknown cipher.

Save results to a file for later reference.

Add a GUI using Tkinter for a graphical interface.

Support other alphabets or languages.

Add a random shift option for stronger basic encryption.

Refactor the repeat logic to use a loop instead of recursion.

📄 License
This project is free to use, modify, and distribute for personal or educational purposes.

