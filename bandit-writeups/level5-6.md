# Bandit Level 5 → 6
The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

human-readable
1033 bytes in size
not executable

---

## 🔹 Get to level 5
1. Open a terminal.  
2. Connect using SSH:  
   ```bash
   ssh bandit5@bandit.labs.overthewire.org -p 2220
3. Put in password:
   `4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw'
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
   find -type f -size 1033c ! -executable
* `find` find all files that fit the description behind it
* `-type f` does find by type: file
* `-size 1033c` finds files that are exactly 1033 bytes (c=bytes)
* `! -executable` means **not** executable
This gave me a path:
`./maybehere07/.file2`

4. To open the path and file `./maybehere07/.file2`, I typed:
    ```bash
    cat ./maybehere07/.file2
  * `cat` shows the contents of a file
  * I used `./` before the name because opening a file name starting with `-` can be problematic. This is because the dash (-) is commonly used to introduce command-line flags or options.
  * `./` is important to use to tell the shell that the file is located in the current working directory
  * this gave me the contents of the file, showing me the password I needed
4. Level 6 password:
`HWasnPhtq9AVKe0dmk45nxy20cvUa6EG`
