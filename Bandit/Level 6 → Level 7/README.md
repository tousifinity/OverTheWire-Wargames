## 🔓 Bandit Level 6 → Level 7

### 🧩 Level Goal

> The password for the next level is stored somewhere on the server and has **all** of the following properties:
> - Owned by **user** `bandit7`
> - Owned by **group** `bandit6`
> - **33 bytes** in size

---

### 🛠 Tools Used

- Linux Terminal
- Linux commands: `find`, `cat`
- Output filtering: `2>/dev/null`

---

### 🪜 Steps to Solve

1. Log in using `bandit6` credentials:

    ```bash
    ssh bandit6@bandit.labs.overthewire.org -p 2220
    # Password: HWasnPhtq9AVKe0dmk45nxy20cvUa6EG
    ```

2. Use the `find` command to search the entire filesystem (`/`) for files:
   - That are **owned by user `bandit7`**
   - That are **owned by group `bandit6`**
   - That are exactly **33 bytes in size**

    Also suppress permission errors by redirecting them to `/dev/null`. 2 refers to **stderr** (standard error stream).

    ```bash
    find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null
    ```

    Output:

    ```
    /var/lib/dpkg/info/bandit7.password
    ```

3. Read the contents of the file:

    ```bash
    cat /var/lib/dpkg/info/bandit7.password
    ```

    Output:

    ```
    morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj
    ```

---

### 🔑 Password for Level 7:
    morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj

