# Bandit Level 3 → 4
## 🔹 Goal
The goal of this level is to find the password in a hidden file in the `inhere` directory.

---

## 🔹 Get to level 3
1. Open a terminal.  
2. Connect using SSH:  
   ```bash
   ssh bandit3@bandit.labs.overthewire.org -p 2220
3. Put in password:
   `MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx'

## 🔹 Steps
1. Type:
   ```bash
   cd ./inhere
  * `cd` changes the directory to the one typed
2. Type:
   ```bash
   ls
* I typed this and did not see any files
3. Typed:
   ```bash
   ls -ld .?*
* `ls` to list files
* `-l` to use long listing format
* `-d` list directory entries instead of contents
* `.?*` to only state hidden files
* it showed:
`-rw-r----- 1 bandit4 bandit3 33 Aug 15 13:16 ...Hiding-From-You`

4. To open the `...Hiding-From-You` file, I typed:
    ```bash
    cat ./...Hiding-From-You
  * `cat` shows the contents of a file
  * I used `./` before the name because opening a file name starting with `-` can be problematic. This is because the dash (-) is commonly used to introduce command-line flags or options.
  * `./` is important to use to tell the shell that the file is located in the current working directory
  * I had to us `'` on either side of the file name because it has spaces in it, so it reads it as one single file name
  * this gave me the contents of the file showing me the password I needed
4. Level 4 password:
`2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ`
