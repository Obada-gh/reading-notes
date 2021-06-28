# Caesar Cipher:
The Caesar Cipher technique is one of the earliest and simplest method of encryption technique. It’s simply a type of substitution cipher, i.e., each letter of a given text is replaced by a letter some fixed number of positions down the alphabet. For example with a shift of 1, A would be replaced by B, B would become C, and so on. The method is apparently named after Julius Caesar, who apparently used it to communicate with his officials. 
Thus to cipher a given text we need an integer value, known as shift which indicates the number of position each letter of the text has been moved down. 
The encryption can be represented using modular arithmetic by first transforming the letters into numbers, according to the scheme, A = 0, B = 1,…, Z = 25. Encryption of a letter by a shift n can be described mathematically as. 

E_n(x)=(x+n)mod\ 26  
(Encryption Phase with shift n)

D_n(x)=(x-n)mod\ 26  
(Decryption Phase with shift n)

![Caesar Cipher](https://media.geeksforgeeks.org/wp-content/uploads/ceaserCipher.png)

example:
```
#A python program to illustrate Caesar Cipher Technique
def encrypt(text,s):
    result = ""
 
    # traverse text
    for i in range(len(text)):
        char = text[i]
 
        # Encrypt uppercase characters
        if (char.isupper()):
            result += chr((ord(char) + s-65) % 26 + 65)
 
        # Encrypt lowercase characters
        else:
            result += chr((ord(char) + s - 97) % 26 + 97)
 
    return result
 
#check the above function
text = "ATTACKATONCE"
s = 4
print "Text  : " + text
print "Shift : " + str(s)
print "Cipher: " + encrypt(text,s)
```

# Encryption, Decryption & Hacking:

A symmetric encryption is any technique where the same key is used to both encrypt and decrypt the data. The Caesar Cipher is one of the simplest symmetric encryption techniques, and of course, one of the easiest to crack.
Since then, cryptologists have invented many more symmetric encryption techniques, including the ones used today to encrypt data like passwords.
Vigenère Cipher
French cryptologists invented the Vigenère Cipher in the mid 1500s. The cipher was considered especially strong, and author Lewis Caroll even called it “unbreakable” in 1868. It was indeed much stronger than the Caesar Cipher, but as we’ll see, it can definitely be cracked.
Encryption
The Vigenère cipher uses an entire word as the shift key, as opposed to the Caesar Cipher’s single shift amount.
Imagine that we want to encrypt the phrase VERSAILLES and use a shift key of CHEESE.
First, we need to repeat the shift key to line up with each of the letters in the phrase:
Original	V	E	R	S	A	I	L	L	E	S
Shift key	C	H	E	E	S	E	C	H	E	E
Now we replace each letter of the original text according to the Vigenère table:

![table](https://i.ibb.co/RCBTYrD/Screenshot-1.png)

Cracking the cipher
Imagine that a very literate and savvy enemy intercepts one of Caesar's messages.
RZ VMZ WMDIBDIB VGG AJMXZN OJ EJDI RDOC XGZJKVOMV OJ YZAZVO OCZ ZIZHT LPZZI VO OCZ IDGZ YZGOV
That enemy does not know that Caesar always uses a shift of 3, so he must attempt to "crack" the cipher without knowing the shift.
There are three main techniques he could use: frequency analysis, known plaintext, and brute force.
Frequency analysis
Human languages tend to use some letters more than others. For example, "E" is the most popular letter in the English language. We can analyze the frequency of the characters in the message and identify the most likely "E" and narrow down the possible shift amounts based on that.
Try it out yourself! Paste the message in the text area below and analyze the frequency graph to identify a possible "E"


