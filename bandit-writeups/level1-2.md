# Bandit Level 1 → 2

## 🔹 Goal
The goal of this level is to find the password in the readme file.

---

## 🔹 Get to level 2
1. Open a terminal.  
2. Connect using SSH:  
   ```bash
   ssh bandit1@bandit.labs.overthewire.org -p 2220
3. Put in password:
   `ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If`

## 🔹 Steps
1. Type:
   ```bash
   ls
  * `ls` is used to list the contents of the directory
  * this pulled up a file called `-`
3. To open the `-` file, I typed:
    ```bash
    cat ./-
  * `cat` shows the contents of a file
  * I used `./` before the name bacause opening a file name staring with `-` can be problematic. This is because the dash (-) is commonly used to introduce command line flags or options.
  * `./` is important to use to tell the shell that the file is loacted in the current working directory 
  * this gave me the contents of the file showing me the password I needed
4. Level 2 password:
`263JGJPfgU6LtdEvgfWU1XP5yac29mFx`

