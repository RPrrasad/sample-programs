Description:
SHA-256 ( Secure Hash Algorithms )
A cryptographic hash also called as ‘digest’ is a kind of ‘signature’ for a text or a data file. SHA-256 belongs to the SHA-2 family of cryptographic hashes. It produces the 256 bit (32-byte) digest of a message. A hash is not ‘encryption’ – it cannot be decrypted back to the original text (it is a ‘one-way’ cryptographic function, and is a fixed size for any size of source text). This makes it suitable when it is appropriate to compare ‘hashed’ versions of texts, as opposed to decrypting the text to obtain the original version.

Features
•	Digital signatures 
•	Anti-tamper 
•	Challenge hash authentication

Requirements
Some variants of it are supported by Python in the “hashlib” library (sha256, sha384, sha224, sha512, sha1, md5). These can be found using “algorithms_guaranteed” function of hashlib.
Ex: print (hashlib.algorithms_guaranteed)

Functions:
encode() : Converts the string into bytes to be acceptable by hash function.
hexdigest() : Returns the encoded data in hexadecimal format.

Implement the Solution
The given code takes string and converts it into the byte equivalent using encode() so that it can be accepted by the hash function.
hashlib.sha256(hash_string.encode() ).hexdigest()
The SHA hash functions encode it and then using hexdigest(), hexadecimal equivalent encoded string is printed.

