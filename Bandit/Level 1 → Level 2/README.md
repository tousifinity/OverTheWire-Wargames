## 🔓 Bandit Level 1 → Level 2

### 🧩 Level Goal

> The password for the next level is stored in a file called `-` located in the home directory.

---

### 🛠 Tools Used

- Lunux Terminal
- Linux commands: `ls`, `cat`, `./` (file handling with special characters)

---

### 🪜 Steps to Solve

1. Log in to the server using the credentials for `bandit1`:

    ```bash
    ssh bandit1@bandit.labs.overthewire.org -p 2220
    # Password: ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If
    ```

2. List the files in the home directory:

    ```bash
    ls
    ```

    Output:

    ```
    -
    ```

    The file name is just a hyphen (`-`), which is usually interpreted as standard input when used in commands like `cat`. So we need to avoid that.

3. Read the contents of the file by specifying its path explicitly using `./` to indicate the current directory:

    ```bash
    cat ./-
    ```

    Output:

    ```
    263JGJPfgU6LtdEvgfWU1XP5yac29mFx
    ```

---

### 🔑 Password for Level 2:
    263JGJPfgU6LtdEvgfWU1XP5yac29mFx
    

