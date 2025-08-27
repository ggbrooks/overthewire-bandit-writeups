# Bandit Level 0

## 🔹 Goal
The goal of this level is to log into the game using SSH.  
We connect to the Bandit server with the provided credentials.

---

## 🔹 Connection Details
- **Host:** `bandit.labs.overthewire.org`  
- **Port:** `2220`  
- **Username:** `bandit0`  
- **Password:** `bandit0`  

---

## 🔹 Steps
1. Open a terminal.  
2. Connect using SSH:  
   ```bash
   ssh bandit0@bandit.labs.overthewire.org -p 2220
3. Put in password:
   `bandit0`

# Bandit Level 0 → 1

## 🔹 Goal
The goal of this level is to find the password in the readme file.

---

## 🔹 Steps
1. Type:
   ```bash
   ls
  * `ls` is used to list the contents of the directory
  * this pulled up a file called `readme`
3. To open the `readme` file, I typed:
    ```bash
    cat readme
  * `cat` shows the contents of a file
  * this gave me the contents of the file showing me the password I needed
4. Level 1 password:
`ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If`

     
