## 🔓 Bandit Level 10 → Level 11

### 🧩 Level Goal

> The password for the next level is stored in the file `data.txt`, which contains **base64 encoded data**.

---

### 🛠 Tools Used

- Linux Terminal
- Linux command: `base64`

---

### 🪜 Steps to Solve

1. Log in using `bandit10` credentials:

    ```bash
    ssh bandit10@bandit.labs.overthewire.org -p 2220
    # Password: FGUW5ilLVJrxX9kMYMmlN4MgbpfMiqey
    ```

2. List the contents of the current directory:

    ```bash
    ls
    ```

    Output:

    ```
    data.txt
    ```

3. Display the contents of `data.txt`:

    ```bash
    cat data.txt
    ```

    Output:

    ```
    VGhlIHBhc3N3b3JkIGlzIGR0UjE3M2ZaS2IwUlJzREZTR3NnMlJXbnBOVmozcVJyCg==
    ```

4. Decode the base64 content to reveal the password:

    ```bash
    cat data.txt | base64 -d
    ```

    Output:

    ```
    The password is dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr
    ```

---

### 🔑 Password for Level 11:
    dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr

