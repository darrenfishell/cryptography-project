---
id: sources-cited
name: Sources Cited
heading: The Pigeonhole
subheading: Principle
image: ""
---

Hash is a function to transform an input of arbitrary length (pre-image) into a fixed-length output through a hash algorithm, and the output is the hash value. This conversion is a kind of Contraction mapping, that is, the space of the hash value is usually much smaller than the space of the input, and different inputs may hash to the same output, so it is impossible to determine the unique input value from the hash value. Simply put, it is a function that compresses a message of any length into a message digest of a fixed length.
One of the common algorithms for hashing is MD5. The principle of the MD5 algorithm can be briefly described as follows: the MD5 code processes the input information in 512-bit groups, and each group is divided into 16 32-bit subgroups. After a series of processing, the output of the algorithm consists of four Composed of 32-bit packets, concatenating these four 32-bit packets will generate a 128-bit hash value.

In the MD5 algorithm, the information needs to be filled first, and this data is supplemented by bit, and the result of the final number of bits modulo 512 is 448. After the data is complemented, its digit length is only 64 bits apart, which is an integer multiple of 512. Even if the number of bits of this data modulo 512 is exactly 448, it must be complemented. The implementation process of the complement: first, add a 1 bit after the data; then add a bunch of 0 bits at the back, until the number of bits of the entire data is modulo 512 and the result is exactly 448. In short, at least 1 bit is added, and at most 512 bits may be added.

<iframe width="560" height="315" src="https://www.youtube.com/embed/5xjMuZIMLLk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
