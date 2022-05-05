---
id: caesar
name: Caesar
heading: A Match
subheading: for Caesar
image: "https://privacycanada.net/app/uploads/2020/01/caesar_cipher.png"
caption: "The Caesar Cipher shifts the message by a set number of characters. <em>Image from <a href='https://privacycanada.net/classical-encryption/caesar-cipher/'>Privacy Canada</a></em>"
---

Caesar cipher is one of the simplest and most widely known encryption techniques. All letters in the plaintext are shifted backwards (or forwards) in the alphabet by a fixed number $$ k $$ and then converted into ciphertext. For example, when the offset is 3, all letters A will be replaced with D, B with E, and so on.

In the case of letters at the end of the alphabet, the cipher wraps back around to the beginning. With an offset of 3, Z would be replaced with C, for example.

The Caesar cipher uses relations between sets. Because all plaintexts are transformed into unique corresponding ciphertexts after function transformation, this is an _injective_ function. You can also produce any plaintext string through the cipher process, so it is _surjective_, as well. Meeting these two conditions, the Caesar cipher is then _bijective_.

The encryption and decryption methods of the Caesar cipher can also be calculated by the mathematical method of congruence. First replace the letters with numbers, `A=0, B=1, ..., Z=25`.

For the encryption method with offset $$ n $$, it is:

$$ E_n(x) = (x + n) mod 26 $$

For decryption:

$$ D_n(x) = (x - n) mod 26 $$

The modulo division ensures the range is always 0 to 25.

With a computer, the Caesar cipher is quite easy to break. We know that the encrypted text starts at a certain letter of the alphabet that is not the plaintext location. As such, the user only needs to iterate over 25 other ways to shift the letters by one position to find the combination that produces the intelligible plaintext.
