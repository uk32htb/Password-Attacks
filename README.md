# Password-Attacks

1) Dictionary Attacks :- Cracking password using pre generated wordlist like rockyou.txt
2) Brute Force Attacks :-
3) Rainbow Table Attacks :- Chekcing the hash alonside pre generated hashes of well known passwords.

======================================================================================================================================================================

1) Single Crack mode:- checking hashes with the hash value 
john --format=<hash_type> <hash or hash_file> :- e.g john --format=sha256 hash.txt


2) Wordlist Crack Mode :- Checking the hashes against the wordlist
john --wordlist=<wordlist_file> --rules <hash_file> :- e.g. john --wordlist=rockyou.txt --rules hash.txt
        Note :- --rule, this will generate password list based on the in built rules. Like adding appending numbers, capitalizing letters and adding special characters.

3) Incremental Mode :- Will read the hashes in the specified hash file and then generate all possible combinations of characters, starting with a single character and incrementing with each iteration. 
