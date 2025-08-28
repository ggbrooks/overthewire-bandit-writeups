# Bandit Level 4 → 5

## 🔹 Goal
The goal of this level is to find the password that is stored in the only human-readable file in the inhere directory.

---

## 🔹 Get to level 4
1. Open a terminal.  
2. Connect using SSH:  
   ```bash
   ssh bandit4@bandit.labs.overthewire.org -p 2220
3. Put in password:
   `2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ'
---

## 🔹 Steps
1. Type:
   ```bash
   cd ./inhere
  * `cd` changes the directory to the one typed
2. Type:
   ```bash
   ls
* I typed this and saw multiple files

3. Typed:
   ```bash
   file ./*
* this checks all of the files and tells me what type it is
* all of them said `data` except for one
* one said `ASCII text`, which tells us this is the only human-readable file: `-file07'

4. To open the `-file07` file, I typed:
    ```bash
    cat ./-file07
  * `cat` shows the contents of a file
  * I used `./` before the name because opening a file name starting with `-` can be problematic. This is because the dash (-) is commonly used to introduce command-line flags or options.
  * `./` is important to use to tell the shell that the file is located in the current working directory
  * this gave me the contents of the file, showing me the password I needed
4. Level 5 password:
`4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw`
