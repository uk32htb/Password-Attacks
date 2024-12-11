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



======================================================================================================================================================================

We can use John to convert any type of file into the hash and crack the password. 

We can check the #locate *2john* to find what files we can convert it to 

locate *2john*

/usr/bin/bitlocker2john
/usr/bin/dmg2john
/usr/bin/gpg2john
/usr/bin/hccap2john
/usr/bin/keepass2john
/usr/bin/putty2john
/usr/bin/racf2john
/usr/bin/rar2john
/usr/bin/uaf2john
/usr/bin/vncpcap2john
/usr/bin/wlanhcx2john
/usr/bin/wpapcap2john
/usr/bin/zip2john
/usr/share/john/1password2john.py
/usr/share/john/7z2john.pl
/usr/share/john/DPAPImk2john.py
/usr/share/john/adxcsouf2john.py
