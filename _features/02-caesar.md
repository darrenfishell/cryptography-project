---
id: caesar
name: Caesar's Code
heading: No Match
subheading: for Caesar
image: "assets/img/caesar-cipher.png"
---

Caesar cipher is one of the simplest and most widely known encryption techniques. All letters in the plaintext are shifted backwards (or forwards) in the alphabet by a fixed number k and then converted into ciphertext. For example, when the offset is 3, all letters A will be replaced with D, B with E, and so on.

## Math behind
The relation between set is used. Because all plaintexts are transformed into unique corresponding ciphertexts after function transformation, this is a bijective function.

The encryption and decryption methods of the Caesar cipher can also be calculated by the mathematical method of congruence. First replace the letters with numbers, A=0, B=1, ..., Z=25.

For the encryption method with offset n, it is:

For decryption:

So, the range is always 0 to 25.