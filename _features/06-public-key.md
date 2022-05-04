---
id: public-key
name: Public Key Cryptography
heading: Public Key
subheading: Cryptography
image: ""
---

The traditional encryption method is to use the same key for encryption and decryption, which is stored by the sender and the receiver respectively and used during encryption and decryption. The main problem with this method is the generation, injection, storage, management and distribution of the key. etc. is complicated, especially as the number of users increases exponentially the demand for keys. In network communication, the distribution of a large number of keys is a difficult problem to solve.

For example, if there are n users in the system, and password communication needs to be established between every two users, each user in the system must master $$ (n-1) $$ keys, and the total number of keys required in the system is $$ n * (n-1)/2 $$. Or $$ _nC_r(n, n-2) $$. This only considers the case where only one session key is used for communication between users.

It is based on this theory that the famous RSA algorithm appeared in 1977. This algorithm provides a basic method for encrypting and authenticating information on public networks. It usually generates a pair of RSA keys first, one of which is a secret key, which is kept by the user; the other is a public key, which can be disclosed to the outside world and even registered in a network server.

When transmitting information, a combination of traditional encryption methods and public key encryption methods is often used, and then the RSA key is used to encrypt the session key and information digest. After receiving the information, the other party decrypts it with a different key and can check the information summary.
