## 🔓 Bandit Level 5 → Level 6

### 🧩 Level Goal

> The password for the next level is stored in a file somewhere under the `inhere` directory and has **all** of the following properties:
>
> - Human-readable
> - Exactly 1033 bytes in size
> - **Not executable**

---

### 🛠 Tools Used

- Linux Terminal
- Linux commands: `find`, `file`, `cat`

---

### 🪜 Steps to Solve

1. Log in using `bandit5`:

    ```bash
    ssh bandit5@bandit.labs.overthewire.org -p 2220
    # Password: 4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
    ```

2. Navigate to the `inhere` directory:

    ```bash
    cd inhere
    ```

3. Use the `find` command to search for a **human-readable, 1033-byte, non-executable file**:

    ```bash
    find . -type f -size 1033c -not -executable
    ```

    Output:

    ```
    ./maybehere07/.file2
    ```

4. Display the content of the file:

    ```bash
    cat ./maybehere07/.file2
    ```

    Output:

    ```
    HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
    ```

---

### 🔑 Password for Level 6:
    HWasnPhtq9AVKe0dmk45nxy20cvUa6EG

