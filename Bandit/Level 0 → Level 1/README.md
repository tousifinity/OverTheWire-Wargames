## 🔓 Bandit Level 0 → Level 1

### 🧩 Level Goal

> The password for the next level is stored in a file called `readme` located in the home directory. Use this password to log into `bandit1` using SSH.

---

### 🛠 Tools Used

- Linux Terminal
- Basic Linux commands: `ls`, `cat`

---

### 🪜 Steps to Solve

1. Log into the Bandit game server using SSH with the credentials for `bandit0`:

    ```bash
    ssh bandit0@bandit.labs.overthewire.org -p 2220
    # Password: bandit0
    ```

2. After logging in, list the files in the home directory:

    ```bash
    ls
    ```

    Output:

    ```
    readme
    ```

3. View the contents of the `readme` file:

    ```bash
    cat readme
    ```

    Output:

    ```
    ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If
    ```

---

### 🔑 Password for Level 1: 
    ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If

