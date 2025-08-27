# Bandit Level 2 → 3
## 🔹 Goal
The goal of this level is to find the password in a file called --spaces in this filename--.

---

## 🔹 Get to level 3
1. Open a terminal.  
2. Connect using SSH:  
   ```bash
   ssh bandit2@bandit.labs.overthewire.org -p 2220
3. Put in password:
   `263JGJPfgU6LtdEvgfWU1XP5yac29mFx'

## 🔹 Steps
1. Type:
   ```bash
   ls
  * `ls` is used to list the contents of the directory
  * this pulled up a file called `--spaces in this filename--`
3. To open the `--spaces in this filename--` file, I typed:
    ```bash
    cat ./'--spaces in this filename--'
  * `cat` shows the contents of a file
  * I used `./` before the name bacause opening a file name staring with `-` can be problematic. This is because the dash (-) is commonly used to introduce command line flags or options.
  * `./` is important to use to tell the shell that the file is loacted in the current working directory
  * I had to us `'` on either side of the file name because it has spaces in it, so it reads it as one single file name
  * this gave me the contents of the file showing me the password I needed
4. Level 3 password:
`MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx`
