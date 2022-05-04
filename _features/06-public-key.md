---
id: public-key
name: Public Key Cryptography
heading: Public Key
subheading: Cryptography
image: ""
---

Traditional encryption uses the same key for encryption and decryption. For this, the sender and receiver must store the same key.

The main problem with this encryption technique method is the generation, injection, storage, management and distribution of the key. This becomes increasingly unwieldy as the number of users increases. In network communication, the distribution of a large number of keys is a difficult problem to solve.

For example, if there are $$ n $$ users in the system, and password communication needs to be established between every pair of users, each user in the system must master $$ (n-1) $$ keys, and the total number of keys required in the system is $$ n * (n-1)/2 $$. Or $$ _nC_r(n, n-2) $$. This only considers the case where only one session key is used for communication between users.

Based on this challenge, the famous RSA algorithm appeared in 1977. This algorithm provides a basic method for encrypting and authenticating information on public networks. It usually generates a pair of RSA keys first, one of which is a secret key, which is kept by the user; the other is a public key, which can be disclosed to the outside world and even registered in a network server.

The basis of RSA encryption is the difficulty of _prime factorization_ of large integers. While there are other components of RSA encryption, the primary keys are identified in the equation $$ p \cdot q = N $$, where $$ p $$ and $$ q $$ are prime numbers.

The product $$ N $$ forms one component of the public key. The other is defined by another mathematical operation called a _totient function_, which is used to define other values $$ d $$ and $$ e $$, representing encryption and decryption keys, respectively.

The decryption key value is kept secret while the encryption value is part of the public key, along with $$ e $$.

When transmitting information, a combination of traditional encryption methods and public key encryption methods is often used, and then the RSA key is used to encrypt the session key and information digest. After receiving the information, the other party decrypts it with a different key and can check the information summary.
