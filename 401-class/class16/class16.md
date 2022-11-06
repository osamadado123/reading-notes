# Encryption, Decryption & Hacking

## Encrypting a message
Imagine Caesar wants to send this message:<br>
SECRET MEETING AT THE PALACE<br>
Here's what that might look like encrypted:<br>
YKIXKZ SKKZOTM GZ ZNK VGRGIK<br>
That looks an awfully lot like gobbledygook at first, but this encrypted message is actually very related to the original text.
The Caesar Cipher is a simple substitution cipher which replaces each original letter with a different letter in the alphabet by shifting the alphabet by a certain amount.
![pic](/401-class/class16/314394794_2398766080276398_2706495651833445861_n.png)

## Decrypting a message
According to historical records, Caesar always used a shift of 3. As long as his message recipient knew the shift amount, it was trivial for them to decode the message.

## Cracking the cipher
Imagine that a very literate and savvy enemy intercepts one of Caesar's messages. <br>
RZ VMZ WMDIBDIB VGG AJMXZN OJ EJDI RDOC XGZJKVOMV OJ YZAZVO OCZ ZIZHT LPZZI VO OCZ IDGZ YZGOV <br>
That enemy does not know that Caesar always uses a shift of 3, so he must attempt to "crack" the cipher without knowing the shift.
There are three main techniques he could use: frequency analysis, known plaintext, and brute force.

# Ceasar Cipher

In cryptography, a Caesar cipher, also known as Caesar's cipher, the shift cipher, Caesar's code or Caesar shift, is one of the simplest and most widely known encryption techniques. It is a type of substitution cipher in which each letter in the plaintext is replaced by a letter some fixed number of positions down the alphabet. For example, with a left shift of 3, D would be replaced by A, E would become B, and so on. The method is named after Julius Caesar, who used it in his private correspondence.