# Substitution Ciphers

It is an elementary encoding technique which involves substituting characters of a plaintext with another character, or perhaps some form of rotation. <br>
<br>
We discuss two of them here:<br>

## Caesar Cipher
Each letter of the plaintext is shifted by a fixed number(known as the *key* of the Caesar cipher) down the alphabet. <br><br>
Example:
```
Plaintext: The quick brown fox jumps over the lazy dog.

Ciphertext with a key of 5: Ymj vznhp gwtbs ktc ozrux tajw ymj qfed itl.
```
All it takes is 25 attempts to figure out the key and decrypt any message.
<br>
## Vigenere Cipher
Instead of a key, it uses a *keyword*. <br>
Algorithm: <br>
1) The keyword is repeated until its length matches that of the plaintext.<br>
2) Let P<sub>i</sub> be each number corresponding to each letter  of the plaintext, and K<sub>i</sub> be that of the keyword. <br>
3) Encryption is defined by : **C<sub>i</sub> = (P <sub>i</sub> + K <sub>i</sub>) mod 26**.
<br><br>
For example:<br>
```
Plaintext: The quick brown fox jumps over the lazy dog.

Ciphertext with keyword 'Shade': Loe tyajk evgdn isp quptk vvhv loe oerf drk.
```
<br>
Decryption:<br>
P<sub>i</sub> = (C<sub>i</sub> - K<sub>i</sub> + 26) mod 26

### Resource: 
https://cryptii.com/ 
