---
id: hash
name: Hashes
heading: Hash
subheading: Functions
image: "https://upload.wikimedia.org/wikipedia/commons/thumb/a/a5/MD5_algorithm.svg/1280px-MD5_algorithm.svg.png"
caption: "This process diagram describes the steps involved in the MD5 hash algorithm. Image from <a href='https://en.wikipedia.org/wiki/MD5'>Wikipedia</a>"
---

A hashing function transforms an input of arbitrary length (pre-image) into a fixed-length output. The output is the _hash value_.

A proper hash function is different than an encryption algorithm in that it should only work in one direction. Like an encryption algorithm, it should also be _collision-free_, or injective, meaning that each input only has one output.

This conversion is a kind of _contraction mapping_, where the hash value is usually much smaller than the input. This generally means that different inputs may hash to the same output, or they are not injective functions.

For cryptography, this is important because it confounds any effort to determine the unique input value from the hash value.

One of the common algorithms for hashing is MD5. The principle of the MD5 algorithm can be briefly described as follows:

* The input information is broken into 512-bit groups
* Each group is further divided into 16 32-bit subgroups.
* Concatenating these four 32-bit packets will generate a 128-bit hash value.

In the MD5 algorithm, the information needs to be padded out to a bit-length $$ x $$ where $$ x \mod 512 = 448 $$.

After the data is complemented, its digit length is only 64 bits apart, which is an integer multiple of 512. Even if the number of bits of this data modulo 512 is exactly 448, it must be complemented.

The implementation process of the complement is as follows: first, add a 1 bit after the data; then add a bunch of 0 bits at the back, until the number of bits modulo 512 is exactly 448. In short, at least 1 bit is added, and at most 512 bits may be added.

Use the following interactive shell to produce an MD5 hash value and a SHA256 hash for the plaintext password below:

{% include_relative datacamp/md5-hash-playground.html %}

Now, let's reproduce the hash multiple times. Moving through just three iterations, we can see that the values are the same in each iteration, for both hash methods:

{% include_relative datacamp/hash-iterations.html %}

