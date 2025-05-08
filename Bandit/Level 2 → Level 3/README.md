## 🔓 Bandit Level 2 → Level 3

### 🧩 Level Goal

> The password for the next level is stored in a file called `spaces in this filename` located in the home directory.

---

### 🛠 Tools Used

- Linux Terminal
- Linux commands: `ls`, `cat`
- Handling filenames with spaces using quotes or escape characters

---

### 🪜 Steps to Solve

1. Log in to the server with `bandit2` credentials:

    ```bash
    ssh bandit2@bandit.labs.overthewire.org -p 2220
    # Password: 263JGJPfgU6LtdEvgfWU1XP5yac29mFx
    ```

2. List the files in the home directory:

    ```bash
    ls
    ```

    Output:

    ```
    spaces in this filename
    ```

3. There are two common ways to access files with spaces in their names:

    - Using quotes:

        ```bash
        cat ./"spaces in this filename"
        ```

    - Or using escape characters (`\`):

        ```bash
        cat spaces\ in\ this\ filename
        ```

4. Either method will display the password.

    Output:

    ```
    MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx
    ```

---

### 🔑 Password for Level 3:
    MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx
