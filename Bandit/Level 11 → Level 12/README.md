## 🔓 Bandit Level 11 → Level 12

### 🧩 Level Goal

> The password for the next level is stored in the file `data.txt`, where all **lowercase (a-z)** and **uppercase (A-Z)** letters have been **ROT13-encoded**.

---

### 🛠 Tools Used

- Linux Terminal
- Command used: `cat`, `tr`

---

### 🪜 Steps to Solve

1. Log in with your Bandit level 11 credentials:

    ```bash
    ssh bandit11@bandit.labs.overthewire.org -p 2220
    # Password: dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr
    ```

2. List the contents of the directory:

    ```bash
    ls
    ```

    Output:

    ```
    data.txt
    ```

3. Check the contents of `data.txt`:

    ```bash
    cat data.txt
    ```

    Output:

    ```
    Gur cnffjbeq vf 7k16JArUVv5LxVuJfsSVdbbtaHGlw9D4
    ```

4. Decode using ROT13:

    ```bash
    cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
    ```

    Output:

    ```
    The password is 7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4
    ```

---

### 🔑 Password for Level 12:
    7x16WNeHIi5YkIhWsfFIqoognUTyj9Q4

