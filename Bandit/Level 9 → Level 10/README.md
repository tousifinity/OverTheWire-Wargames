## 🔓 Bandit Level 9 → Level 10

### 🧩 Level Goal

> The password for the next level is stored in the file `data.txt` in **one of the few human-readable strings**, preceded by several `=` characters.

---

### 🛠 Tools Used

- Linux Terminal
- Linux commands: `strings`, `grep`

---

### 🪜 Steps to Solve

1. Log in using `bandit9` credentials:

    ```bash
    ssh bandit9@bandit.labs.overthewire.org -p 2220
    # Password: 4CKMh1JI91bUIZZPXDqGanal4xvAg0JM
    ```

2. List the contents of the current directory:

    ```bash
    ls
    ```

    Output:

    ```
    data.txt
    ```

3. Use the `strings` command to extract human-readable content from the binary file and `grep` to filter lines that contain `=`:

    ```bash
    strings data.txt | grep '='
    ```

    Output:

    ```
    ......
    ......
    ========= FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey
    ......
    ......
    ```

4. The line that seems most likely is the one that contains a clear human-readable string:

    ```
    ========= FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey
    ```

---

### 🔑 Password for Level 10:
    FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey

