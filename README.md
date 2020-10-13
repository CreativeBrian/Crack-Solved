# Crack-Solved
This application reverses an MD5 hash using a brute force technique where we simply 'forward hash' all possible combinations of characters in strings. 
This is similar to a situation where an e-commerce site stored hashed passwords in its database and we somehow have gotten our hands on the database contents and we want to take the hashed password and determine the actual plaintext passwords.

This application takes an MD5 value like "81dc9bdb52d04dc20036dbd8313ed055" (the MD5 for the string "1234") and check all combinations of four-digit "PIN" numbers to see if any of those PINs produce the given hash.

The user is presented with a form where they can enter an MD5 string and request it to reverse-hash the string. If the reverse hash of the string is successful, the application prints out the PIN:

PIN: 1234

If the string does not reverse hash to a four digit number, the application outputs a message like:

PIN: Not found

This application also prints out the first 15 attempts to reverse-hash including both the MD5 value and PIN that you were testing and also prints out the elapsed time for the computation.
