## Caesar Cipher
A command-line Caesar cipher written in Python. It uses a list of the alphabet and a shift number to encrypt or decrypt text, and keeps prompting until the user chooses to stop.

## Features
Encrypt — Shifts each letter forward by the given amount to produce encrypted text.

Decrypt — Shifts each letter backward by the given amount to recover the original text.

Non-Letter Handling — Leaves spaces, punctuation, and digits unchanged while shifting only letters.

Shift Wrapping — Uses modulo 26 so any shift number (including large ones) wraps correctly around the alphabet.

Mode Validation — Re-prompts until the user enters e or d.

Shift Validation — Re-prompts until a valid whole number is entered.

Try Again — Recursively restarts the process if the user answers y.

## Technologies Used
| Technology | Purpose |
|---|---|
| Python | Application logic |
| List (`alphabet`) | Defines the letters used for shifting |
| `alphabet.index()` | Finds each letter's position |
| Modulo (`% 26`) | Wraps the shift around the alphabet |
| `input()` / `print()` | Console interaction |
| `int()` | Parses the shift number |
| `try / except` | Handles invalid shift input |
| Recursion | Restarts the cipher via `caesar()` |
<!-- -->
## How to Use It
Install Python 3.6 or newer from python.org and make sure it's added to your PATH.

Save the code as caesar.py.

Open a terminal in the folder containing the file.

Run python caesar.py.

Choose e to encrypt or d to decrypt, enter your message, enter a shift number, and answer y or n when asked to try again.

## Improvements
Use a loop instead of recursion — caesar() calls itself every time the user retries, which stacks frames and will eventually hit Python's recursion limit after enough runs; a while True loop is safer.

Keep the original case — the text is lowercased before processing, so Hello becomes hello; detecting uppercase letters and preserving their case would make the output cleaner.
