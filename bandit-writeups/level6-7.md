# Bandit Level 6 → 7
The password for the next level is stored somewhere on the server and has all of the following properties:

owned by user bandit7
owned by group bandit6
33 bytes in size
---

## 🔹 Get to level 6
1. Open a terminal.  
2. Connect using SSH:  
   ```bash
   ssh bandit6@bandit.labs.overthewire.org -p 2220
3. Put in password:
   `HWasnPhtq9AVKe0dmk45nxy20cvUa6EG'
---

## 🔹 Steps
1. Type:
   ```bash
   find / -type f -size 33c -user bandit7 -group bandit6 2>/dev/null
* `-type f` shows regular files only
* `-size 33c` show files where size is 33 bytes (c=bytes)
* `-user bandit7` file owner is bandit7
* `-group bandit6` file group is bandit6
* `2>/dev/null` this is important because it hides permission-denied noise
* the path it gave me: `/var/lib/dpkg/info/bandit7.password`
2. Type:
   ```bash
   cat /var/lib/dpkg/info/bandit7.password
* It gave me the password

3. Level 7 password:
`morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj`
