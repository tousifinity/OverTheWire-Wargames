## 🔓 Bandit Level 8 → Level 9

### 🧩 Level Goal

> The password for the next level is stored in the file `data.txt` and is the **only line of text that occurs only once**.

---

### 🛠 Tools Used

- Linux Terminal
- Linux commands: `sort`, `uniq`

---

### 🪜 Steps to Solve

1. Log in using `bandit8` credentials:

    ```bash
    ssh bandit8@bandit.labs.overthewire.org -p 2220
    # Password: dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc
    ```

2. List the contents:

    ```bash
    ls
    ```

    Output:

    ```
    data.txt
    ```

3. Use the following command to sort the data and extract only the **unique** line:

    ```bash
    sort data.txt | uniq -u
    ```

    Output:

    ```
    4CKMh1JI91bUIZZPXDqGanal4xvAg0JM
    ```

---

### 🔑 Password for Level 9:
    4CKMh1JI91bUIZZPXDqGanal4xvAg0JM

