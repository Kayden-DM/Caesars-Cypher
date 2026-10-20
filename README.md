Caesar Cipher
A command-line Python program that encrypts or decrypts messages using a Caesar cipher with a user-chosen shift value.

Concepts Used
Functions — the cipher logic and input validation are separated into reusable functions.

Modulo Arithmetic — (position + shift) % 26 wraps the alphabet so shifts stay in range.

Recursion — caesar() calls itself when the user chooses to try again.

Features
Encrypt & Decrypt — shift letters forward to encrypt or backward to decrypt.

Input Validation — loops until a valid mode (e/d) or whole-number shift is entered.

Non-Letter Handling — spaces, punctuation, and digits pass through unchanged.

Improvements
Replace Recursion with a Loop — repeated "try again" calls keep stacking frames; a while loop is safer.

Preserve Original Case — lowercasing the message loses capitals; handle upper and lower case separately.

Support Larger Shifts — % 26 is already applied, but negative input could be rejected or clearly explained for clarity.
