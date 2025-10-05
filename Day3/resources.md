# Cryptography
Hi guys, going onto the domain of Cryptography.

### Ciphers

1. **Caesar Cipher**: Shifts each letter in the plaintext by a fixed number of positions in the alphabet. **Most famous is shifting by 13 alphabets.** Look up **ROT13**.
2. **Vigenère Cipher**: Uses a keyword to shift letters in the plaintext by varying amounts.
3. **XOR Cipher**: Encrypts data by applying the XOR operation with a key.

### Encodings

1. **Base64**: Encodes binary data into ASCII text using a set of 64 characters for safe transmission. **Usually ends with 1 to 3 `=`s .**
2. **Base58**: Similar to Base64 but omits confusing characters, used in Bitcoin addresses.
3. **Base32**: Encodes binary data into ASCII text using a set of 32 characters, often used for QR codes.
These are some of the **Base Encodings**.

### Encryption
What really is [Encryption](https://cloud.google.com/learn/what-is-encryption)?
There are mainly two types of encryption:
1. **Symmetric** encryption: Message is encrypted using a **key** and decrypted using the **same key**. Eg. AES, DES
2. **Assymetric** encryption: Encryption and decryption happens using two **different keys**. Eg. RSA

When learning about different algorithms that are being used in real-life applications **be sure to read about why/why not they are being used, their pros and cons**. I also like to read about their **history**.

Coming onto algorithms we will be mainly talking about RSA:
1. [**RSA (Rivest-Shamir-Adleman)** ](https://www.geeksforgeeks.org/rsa-algorithm-cryptography/): An **asymmetric** encryption algorithm that uses a public key for encryption and a private key for decryption, widely used for secure data transmission and digital signatures.

### Hashing
Now what is this thing :/ ? 
Encryption as you may have noticed, is **two-way**. It can be decrypted to obtain the original message that was encrypted.
Hashing **cannot be reversed** to obtain the original message that was hashed. It is **one-way**.

- [**Hash Functions**](https://hackmd.io/@ZkRVcTfbTiiU3lJHNmu6ww/BJMK-Lbwxe)
- SHA Family of hash functions: [Link](https://en.wikipedia.org/wiki/Secure_Hash_Algorithms)


### Tools 
- [CyberChef](https://gchq.github.io/CyberChef/)
- [dCode](https://dcode.fr)
- QuipQiup (https://quipqiup.com)
- Hash Analyser (https://www.tunnelsup.com/hash-analyzer/)
---

NOTE: One can confuse terms like Cipher/Encoding/Encryption with each other (i did ToT). They aren't same. 
[Encoding vs Encryption](https://www.geeksforgeeks.org/computer-networks/difference-between-encryption-and-encoding/)

**PS:** Some of the other encryption I like are Salsa20, Chacha20.
Fun fact, the encryption flowchart of these two **actually resemble the salsa dance form**.

---

**PS:** Cryptography, in my opinion is a comparatively harder domain. So it would enough if you would just go through all this. We will send some easier challenges. 
There's a lot of maths associated with cryptography. No need to dive into that for now. 
Cryptography is pretty fun. Read about the algos. It's fun learning about who cracked which algorithm, how did they crack it. Above all, Learnathon is not just about one's interest in learning. ***So learn and enjoy your vacations.***

***Happy learning guys!!***




