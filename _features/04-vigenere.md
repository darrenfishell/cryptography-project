---
id: vigenere
name: Vigenère
heading: Vigenère's
subheading: Cipher
image: "https://upload.wikimedia.org/wikipedia/commons/thumb/9/9a/Vigen%C3%A8re_square_shading.svg/1280px-Vigen%C3%A8re_square_shading.svg.png"
caption: "The Vigenère square, or table, is used along with a key to encode and decode messages. Image from <a href='https://en.wikipedia.org/wiki/Vigen%C3%A8re_cipher'>Wikipedia</a>."
---

The Vigenère cipher uses an alphabetical grid and a keyword to encode and decode messages.

The table (shown in the figure) consists of 26 lines of the alphabet, each of which is obtained by offsetting the previous line one bit to the left. Which line of the alphabet to use for compilation is based on the key, and it changes constantly during the process.

For example, suppose the plaintext is: ATTACKATDAWN

Select a keyword and repeat it to generate a key that is the same length as the plaintext. For example, when the keyword is LEMON, the key is: LEMONLEMONLE.

This key serves as a guide for which row of the alphabetical grid to use when encoding or decoding a message.

In this case, the first letter A of the plaintext corresponds to the first letter L of the key. So, using the L-row of the table, we identify the letter that corresponds to A in the columns, giving us L for the first letter of our ciphertext.

For the second letter, we move to the E row, based on our key, and then move across the columns until we arrive at T, the second letter in our plaintext. The intersection in our grid is X, which is the second letter of our ciphertext.

And so on, you can get:

* Plaintext: ATTACKATDAWN
* Key: LEMONLEMONLE
* Ciphertext: LXFOPVEFRNHR

The introduction of a key here adds a good deal of complexity to the cipher. For instance, by changing our key to ROAST, our ciphertext would then be: RHTSVBOTVTNB.

Changing the key to BREAKNECK, our ciphertext would then be: BKXAMXEVNBNR.
