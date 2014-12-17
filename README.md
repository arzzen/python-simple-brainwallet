Brainwallet [![Build Status](https://travis-ci.org/arzzen/python-simple-brainwallet.svg)](https://travis-ci.org/arzzen/python-simple-brainwallet)
======================

A brainwallet refers to the concept of storing Bitcoins in one's own mind by memorization of a passphrase. As long as the passphrase is not recorded anywhere, the Bitcoins can be thought of as existing nowhere except in the mind of the holder. If a brainwallet is forgotten or the person dies or is permanently incapacitated, the Bitcoins are lost forever.

A brainwallet is created simply by starting with a unique phrase. The phrase must be sufficiently long to prevent brute-force guessing - a short password, a simple phrase, or a phrase taken from published literature is likely to be stolen by hackers who use computers to quickly try combinations. A suggestion is to take a memorable phrase and change it in a silly way that is difficult to predict.

The phrase is turned into a 256-bit private key with a hashing or key derivation algorithm (example: SHA256). That private key is then used to compute a Bitcoin address, or a deterministic sequence of addresses. 


Dependences:
======================
* ecdsa 
* hashlib
* binascii
* sys


Usage:
======================
```
python addressgen.py "passphrase"
```

Example:
======================
```
root@pc:~/python addressgen.py "passphrase"
pass phrase: passphrase
private key: 1e089e3c5323ad80a90767bdd5907297b4138163f027097fd3bdbeab528d2d68
BTC address: 13YXiHAXcR7Ho53aExeHMwWEgHcBaAD7Zk

```

