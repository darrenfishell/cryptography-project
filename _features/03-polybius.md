---
id: polybius
name: Polybius
heading: The Polybius
subheading: Cipher
image: "https://media.geeksforgeeks.org/wp-content/uploads/polybius-square.png"
# caption: "Sample caption. <em>Image from <a href="https://www.geeksforgeeks.org/polybius-square-cipher/">geeksforgeeks.com</a></em>"
---

The Polybius cipher uses an alphabet arranged in a chessboard pattern to encrypt and decrypt messages. Using this grid, the texts can be expressed in the form of coordinates. The letter is the ciphertext, and the plaintext is the coordinates of the letter. Polybius Square is a matrix with 6 rows and 6 columns.

The rows are numbered 1-5, as are the columns. There are 26 letters in the table. Except I and J, each letter occupies its own cell. Each letter is then encoded as a coordinate, with the row number presented first.

For example, the word _password_ becomes 35 11 43 43 52 34 42 14 after being encrypted using the Polybius cipher.

The cipher originated using the Greek alphabet, using just 24 letters, meaning that each letter would have its own unique coordinate, with one blank cell.

For the combination of I/J, the decoder would simply need to note both possibilities and then use the context of the rest of the word to determine which letter the sender actually intended.

Another version of this cipher scrambles the order of the initial letters, using a key. For instance, if we were to use our prior key of LEMON, these letters would fill our first row.

The rest of the grid would then be filled by the remaining letters, without duplicates, in alphabetical order. The second line would then be ABCDF, since the fifth letter E is already used in LEMON.
