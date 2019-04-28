# quick_hash
Tested on debian 8 with python 2.7.

Check a hashed password against a provided word list.

Usage:  quick_hash.py [path-to-wordlist] [hashed-password]

Script will run [hashed-password] against the contents of the supplied wordlist by checking
every line in the file using md5, sha1, sha224, sha256, sha512, and LM hashing algorithms.

If a match is found, the "unhashed" plaintext password and hash algorithm used to find it will be presented.

To hash a string from terminal: echo -n qwerty | md5sum
