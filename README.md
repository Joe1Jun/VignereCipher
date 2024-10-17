# Vigenère Cipher in Java

This repository contains a Java implementation of the Vigenère cipher, a method of encrypting alphabetic text by using a simple form of polyalphabetic substitution.

## Overview

The Vigenère cipher encrypts text by applying a keyword, where each letter of the keyword corresponds to a shift in the alphabet. This project includes the main encryption and decryption functionalities along with a sample text processing application.

## Project Structure

- `src/atu/ie/sw/`
  - `ElegyProcessor.java`: Processes a text file, encrypting its contents using a specified keyword and saving the output to a new file.
  - `Runner.java`: Demonstrates the encryption and decryption process with a sample plaintext and the keyword.
  - `Vignere.java`: Contains the core functionality for encrypting and decrypting text using the Vigenère cipher algorithm.

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/Joe1Jun/VignereCipher.git
2. Navigate to the project directory:
   ```bash
   cd VignereCipher
3. Compile the Java files:
   ```bash
   javac src/atu/ie/sw/*.java
4. Run the Runner class to see a sample encryption and decryption:
   ```bash
   java src/atu/ie/sw/Runner
5. To process a text file (elegy.txt), run the ElegyProcessor class:
   ```bash
   java src/atu/ie/sw/ElegyProcessor
## Example

### Encryption

To encrypt a plaintext message, use the `encrypt` method from the `Vignere` class:

```java
Vignere cipher = new Vignere();
String plaintext = "HELLO";
String keyword = "KEY";
String encrypted = cipher.encrypt(plaintext, keyword);
System.out.println("Encrypted: " + encrypted);

```
### Decryption

To decrypt an encrypted message, use the `decrypt` method:

```java
String decrypted = cipher.decrypt(encrypted, keyword);
System.out.println("Decrypted: " + decrypted);

