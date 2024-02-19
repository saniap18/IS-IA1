A brute-force attack is a cryptographic attack that tries every possible combination of characters until the correct password is found. This attack method is straightforward and exhaustive because it does not rely on prior knowledge about the password. It iterates through all possible character combinations until it discovers the correct one.

A brute-force attack can be used to crack hashed passwords. The basic idea is to hash each candidate password using the same hashing algorithm used to create the stored password hashes. These generated hashes are then compared against the target hashes to identify matches. However, brute force attacks are time consuming and not ideal for complex or lengthy passwords.


Brute force attack command example: 'hashcat -a 3 -m 0 hashedpasswords.txt ?u?l?s?d'

-a 3: Brute force attack

-m 0: MD5

hashedpasswords.txt: text file with hashed passwords

?u: looks for an Uppercase letter
?l: looks for a Lowercase letter
?s: looks for a Special character
?d: looks for numbers
These are used to specify the format of the password we're searching for. A password that matches this format could be: 'Sp$1'

When you run the command, Hashcat will search the text file and if the password is found it will return the 'hash value: Password'
