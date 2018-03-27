# Glossary of Blockchain

### Hash

* https://simple.wikipedia.org/wiki/Cryptographic_hash_function

A hash is a sequence of letters and numbers that represent a unique piece of content. The hash is much shorter then the entire content, but any change in the content results in a new hash. This allows for an ID to unique pieces of content. Hashes are one-way however and you can't figure out what the content was based on the hash.

### Public/Private keypair (assymetric cryptography)

* https://www.theatlantic.com/magazine/archive/2002/09/a-primer-on-public-key-encryption/302574/
* https://blogs.msdn.microsoft.com/plankytronixx/2010/10/22/crypto-primer-understanding-encryption-publicprivate-key-signatures-and-certificates/

A lot of what you read about re: wallets for cryptographic currencies revolves around the idea of public and private keypairs. These are a special form of cryptography that let you encrypt with one key and decrypt with one key. It also allows you to "sign" (more on that later) with a private key and verify a signature (more later) using the public key.

Imagine you have 2 keys. You have one that you can freely give to the world (the public one). You have to keep the private key secret. Now anyone in the world can verify (mathematically) that a message came from you (if it was signed by the private key). They can also send you secret messages that only you can decrypt (by using the public key to encrypt a message).

### Byzantine Fault Tolerance

* https://en.wikipedia.org/wiki/Byzantine_fault_tolerance

This is a theorem of computing which means that your system can continue to operate even if some percentage of the nodes participating are *actively* trying to subvert your system. It has been proven that no system may tolerate more than 1/3 of the participants being evil.

This concept is the crux of *all* public (and private) chains. Everyone needs their system to "be byzntine fault tolerant."
