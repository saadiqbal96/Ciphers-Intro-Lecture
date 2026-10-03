# Ciphers-Intro-Lecture (Work in Progress...)

**Encryption**

Encryption was introduced in order to communicate safely over the Internet.
*What encryption is*: plaintext (which basically contains the private information that needs to be sent confidentially) is encrypted and then made unreadable (cypher text) turning it into a string of numbers/letters, and can only be read as plaintext data again by those who have the decryption key.

There are two main ways of communicating through encryption:
- Private (symmetric): in this communication both the sender and receiver use one shared decryption key.
- Public (asymmetric): the sender encrypts plaintext using the receiver public key (lock) in this form of communication the receiver who is identified by the public key is the only one who knows the private key (unlock) and can use it to decrypt the data.

**Symmetric Encryption:**
As said, symmetric encryption uses a single shared key to encrypt and decrypts data. Both Alice and Bob must possess the same secret key before they can communicate securely.
For example, Alice encrypts a message using a shared key and sends it to Bob. Bob then uses that same key to decrypt and read the message.
The main advantage of symmetric encryption is that it is fast and efficient, making it suitable for encrypting large amounts of data.
*Examples:* AES, DES..

**Asymmetric Encryption:**
Asymmetric encryption uses a pair of keys: a public key and a private key.
Bob shares his public key with Alice while keeping his private key secret. Alice encrypts a message using Bob's public key, and only Bob can decrypt it using his private key.
This removes the need to share a secret key beforehand and makes secure communication possible between parties who have never met.
*Examples:* RSA, ECC..

**Alice and Bob Example**
1. Bob generates a public and private key pair.
2. Bob shares his public key with Alice.
3. Alice encrypts a message using Bob's public key.
4. Alice send the encrypted message to Bob.
5. Bob decrypts the message using his private key.

*Only Bob can read the message because only Bob possesses the private key.*
