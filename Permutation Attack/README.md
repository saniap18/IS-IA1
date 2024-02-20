In Hashcat, a combination permutation attack is a type of attack that involves trying various combinations of characters from a given character set to crack passwords. This attack is often used when passwords are created by combining multiple words or elements. The combination permutation attack is achieved through the use of rules in Hashcat.

Command Example: hashcat -a 1 -m 0 md5.txt rockyou.txt rockyou.txt

-a 1: Combination attack

-m 0: MDS 

dictionary file: rockyou.txt

This attack will find permutatations of the passwords in both wordlists. In this example, the combinations of the words will be created with itself
