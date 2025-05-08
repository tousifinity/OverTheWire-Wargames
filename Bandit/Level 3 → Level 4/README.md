## 🔓 Bandit Level 3 → Level 4

### 🧩 Level Goal

> The password for the next level is stored in a hidden file in the `inhere` directory.

---

### 🛠 Tools Used

- Linux Terminal
- Linux commands: `ls`, `ls -a`, `cd`, `cat`

---

### 🪜 Steps to Solve

1. Log in with the credentials for `bandit3`:

    ```bash
    ssh bandit3@bandit.labs.overthewire.org -p 2220
    # Password: MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx
    ```

2. Navigate to the `inhere` directory:

    ```bash
    cd inhere
    ```

3. List all files, including hidden ones:

    ```bash
    ls -a
    ```

    Output:

    ```
    .  ..  ...Hiding-From-You
    ```

4. Read the contents of the hidden file:

    ```bash
    cat ./...Hiding-From-You
    ```

    Output:

    ```
    2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
    ```

---

### 🔑 Password for Level 4:
    2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
    
