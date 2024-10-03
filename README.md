# Password_checker
### Uses an API to access a database of hacked passwords to check if a given password has been leaked.  
The program hashes the password locally using [hashlib](https://docs.python.org/3/library/hashlib.html) and sends a request to the database for all the hashes that start with the same five characters, avoiding sharing the complete hash. Then, the program fetches the complete hash locally; if it is found, the password has been leaked.
