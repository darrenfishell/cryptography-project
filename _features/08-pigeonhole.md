---
id: pigeonhole
name: Pigeonhole
heading: The Pigeonhole
subheading: Principle
image: ""
---

Software engineers typically want to prepare for any scenario, so there's a preference for functions and programs that have an infinite domain of inputs. Hash functions map these inputs to a finite output, or codomain.

This means that there's the possibility that two entirely different inputs will result in the same output, a weakness identified in the MD5 algorithm that makes it susceptible to a specific type of attack using the pigeonhole principle.

The pigeonhole principle states that given $$ n $$ pigeons placed in $$ k $$ holes, if $$ n > k $$ then at least one hole must have more than one pigeon. In fact, we can say that at least one hole must have at least $$ \lceil n/k \rceil $$, rounding up to the next integer.

Following the pigeonhole principle, since our range $$ n $$ is smaller than our domain $$ m $$, it follows that at least one collision must exist. An effective hash function looks only to minimize the number of collisions, but this complicates their use for cryptographic applications, as they are no longer secure.

While the functions were initially created for speed in database upkeep and management, a special branch of hash functions that prioritized privacy, security, & transparency were developed for other uses, called cryptographic hashing functions.

A requirement for hash functions is that it cannot be reversed, so the hash value cannot be used to generate the original input.

Such hash functions are commonly used to store and validate passwords. In these scenarios, when a user submits their password for authentication, the password is then hashed and compared with the stored hash, rather than the actual password.

Increasingly, these hash functions are "salted," which means adding randomnness to the password to further complicate attacks such as the frequency analysis mentioned earlier.

"Salting" a hash algorithm involves concatenating the plaintext with randomized information, which means plaintext of the same value would actually have different hashes. These "salted" values are randomly generated each time a user modifies a password, meaning that they are consistent for a given user but unique across all users.

We can mimic this by generating a random 10-character string and then performing the same hash as we did above. Iterating through three times, we can see the hash values now change with each pass.

{% include_relative datacamp/salted_hash.html %}

Should anyone receive the database of stored, hashed passwords, this makes it much more difficult to identify any patterns among those passwords, as one would do with a frequency analysis that could limit the pool of likely passwords for any given hash.
