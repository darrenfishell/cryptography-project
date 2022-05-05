---
id: cipher-security
name: Security
heading: Balancing Security
subheading: and Efficiency
image: ""
---

The security of a hash algorithm is often at odds with speed and efficiency. This creates a dilemma as hash algorithms play an increasingly large role in our lives and, as a result, have a broader real-world impact.

In Caesar's day, his ciphers didn't take much more than a little brainspace.

Modern hash algorithms are constantly used today to authenticate billions of users of online services.

They are also used as a critical component of increasingly valuable cryptocurrencies and non-fungible tokens.

The Bitcoin consensus mechanism is based on Proof of Work (PoW), where energy is used to keep the blockchain running securely.

"PoW" is the accounting method of digital currency. The so-called "proof-of-work" is to complete the verification and confirmation of the transaction in a very short period of time through the voting of special nodes. For a transaction, if several nodes with unrelated interests can reach a consensus, the entire network can reach a consensus on this transaction.

Miners repeatedly insert bundles of unverified transactions into the hash function, along with a value called a "nonce" and a timestamp of the transaction, until the result meets a current difficulty requirement. The number of such trials per second is called the "hash rate" and is recalibrated to ensure an average of 10 minutes elapses between the addition of successive blocks.

Whoever first calculates the correct answer of the random hash function and submits it receives a reward. There are no tricky solutions to these problems. The computer can only use enumeration until it has an answer.

These calculations are meaningless by themselves, just a proof-of-work. However, it is nearly impossible to put fake transactions in without detection because, in theory, it would require more computing power than everyone else combined.
