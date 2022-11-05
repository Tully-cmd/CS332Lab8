# LAB 8 - Post Exploitation/Cracking Hashes

Target IP: 

1. On your Kali machine, open a terminal window and browse to the location of the `user_logins.txt` file. 

2. John the Ripper has a bunch of rules for common password permutations based on usernames that could potentially crack some of the passwords. To list the available rule list type the following command: 

	`john --list=rules`

3. What is the output of the command? (include screenshot).

4. Use the the "--single" rule to crack the hashes by using the following command: 

	`john --single user_logins.txt`

5. What is the password for the following users:

	- user
	- msfadmin
	- service

6. While John the ripper did reveal the password for some of the users using the "single" rule, it did not crack the password for all the users. We will now use a dictionary list to crack even more passwords. 

7. Type the following command:

	`john --wordlist=/usr/share/john/password.lst --rules user_logins.txt`

8. What does the `--wordlist=/usr/share/john/password.lst` do? 

9. What does the `--rules` option do?

10. What is the password for 'sys' user? 

11. What is the password for 'klog' user?

12. What command would you use to have john display all the passwords you have cracked for user_logins.txt?
