# XOR in Crypto
The XOR operator is very important and frequently used all over cryptography.<br>
## Logical XOR
It has the following truth table: <br><br>
1 XOR 0 = 1<br>
0 XOR 1 = 1<br>
0 XOR 0 = 0<br>
1 XOR 1 = 0<br>
<br>
## XOR Properties
Identical numbers or strings xorred with each other = 0.<br>
<br>
**Commutative**: A XOR B = B XOR A <br>
<br>
**Associative**: A XOR (B XOR C) = (A XOR B) XOR C<br>
<br>
**If, <br>
A XOR B = C<br>
Then,<br>
B = C XOR A<br>
And, A = C XOR B**
<br><br>
## XORing A Plaintext With A Number
XORing byte strings with a number implies you are XORing each byte one after the other with that number to generate a new byte string. <br><br>
For example:<br>
```
String S = "I have a cat."
X = 7
S XOR X = "N'ofqb'f'dfs)"
```
## XORing A Plaintext with Another Plaintext
Repeat the shorter plaintext till it matches the length of the longer one.<br>
XOR each byte of the two plaintexts at every position to generate the new string.<br>
<br>
For example:<br>
```
s1 = b"I have a cat"  // Byte string
s2 = b"dog"
s1 XOR s2 = b'-O\x0f\x05\x19\x02D\x0eG\x07\x0e\x13'
```
<br>
You should be able to tackle any XOR decryption challenge now.



