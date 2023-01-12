# Cryptography

## Encryption, Decryption & Hacking

- One of the earliest encryption techniques is the Caesar Cipher, invented by Julius Caesar more than two thousand years ago to communicate messages to his allies.
- The Caesar Cipher is a great introduction to encryption, decryption, and code cracking, thanks to its simplicity.
- **Frequency analysis** - Human languages tend to use some letters more than others. For example, "E" is the most popular letter in the English language. We can analyze the frequency of the characters in the message and identify the most likely "E" and narrow down the possible shift amounts based on that.
- **Known plaintext** - Another term for the original unencrypted message is plaintext. If the enemy already knew some part of the plaintext, it will be easier for them to crack the rest of the encrypted version.
- **Brute force** - There are only 25 possible shifts (not 26 — why not?). The enemy could take some time to try out each of them and find one that yielded a sensible message. They wouldn't even need to try the shifts on the entire message, just the first word or two.
- The three key aspects of data encryption:
  - Encryption: scrambling the data according to a secret key (in this case, the alphabet shift).
  - Decryption: recovering the original data from scrambled data by using the secret key.
  - Code cracking: uncovering the original data without knowing the secret, by using a variety of clever techniques.
- Whenever we consider a possible encryption technique, we need to think about all those aspects: how easy is it to encrypt? how easy is it to decrypt? And most importantly, how easy is it for a nefarious individual to crack the code?
### Things I want to know more about

- I'd like to know another common cipher to see a separate easy to understand example throughout history.
### Sources

- <https://www.khanacademy.org/computing/computers-and-internet/xcae6f4a7ff015e7d:online-data-security/xcae6f4a7ff015e7d:data-encryption-techniques/a/encryption-decryption-and-code-cracking>
- <https://en.wikipedia.org/wiki/Caesar_cipher>
- <https://www.youtube.com/watch?v=jhXCTbFnK8o>

[Back To Home](../README.md)