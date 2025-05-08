## 🔓 Bandit Level 7 → Level 8

### 🧩 Level Goal

> The password for the next level is stored in the file `data.txt`, **next to the word "millionth"**.

---

### 🛠 Tools Used

- Linux Terminal
- Linux commands: `grep`

---

### 🪜 Steps to Solve

1. Log in using `bandit7` credentials:

    ```bash
    ssh bandit7@bandit.labs.overthewire.org -p 2220
    # Password: morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj
    ```

2. List the contents of the current directory:

    ```bash
    ls
    ```

    Output:

    ```
    data.txt
    ```

3. Use `grep` to find the line containing the word "millionth":

    ```bash
    grep millionth data.txt
    ```

    Output:

    ```
    millionth       dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc
    ```

4. The password is the second column in that line.

---

### 🔑 Password for Level 8:
    dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc

