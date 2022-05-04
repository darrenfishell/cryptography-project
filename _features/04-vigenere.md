---
id: vigenere
name: Vigenère
heading: Vigenère's
subheading: Cipher
image: "assets/img/vigenere.png"
---
_Image: From Wikipedia_

To generate the password, the tabular method needs to be used. The table (shown in the figure) consists of 26 lines of the alphabet, each of which is obtained by offsetting the previous line one bit to the left. Which line of the alphabet to use for compilation is based on the key, and it changes constantly during the process.

For example, suppose the plaintext is: ATTACKATDAWN

Select a keyword and repeat to get the key. For example, when the keyword is LEMON, the key is: LEMONLEMONLE

The first letter A of the plaintext corresponds to the first letter L of the key, so use the L-line alphabet in the table to encrypt to obtain the first letter L of the ciphertext. Similarly, the second letter of the plaintext is T, and the corresponding E row is used for encryption in the table to obtain the second letter X of the ciphertext.

And so on, you can get:

* Plaintext: ATTACKATDAWN
* Key: LEMONLEMONLE
* Ciphertext: LXFOPVEFRNHR
