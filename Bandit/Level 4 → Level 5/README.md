## 🔓 Bandit Level 4 → Level 5

### 🧩 Level Goal

> The password for the next level is stored in the only **human-readable** file in the `inhere` directory.  
> 💡 Tip: If your terminal is messed up, try the `reset` command.

---

### 🛠 Tools Used

- Linux Terminal
- Linux commands: `ls`, `file`, `cat`

---

### 🪜 Steps to Solve

1. Log in using `bandit4`:

    ```bash
    ssh bandit4@bandit.labs.overthewire.org -p 2220
    # Password: 2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ
    ```

2. Go into the `inhere` directory:

    ```bash
    cd inhere
    ```

3. List all files in the directory:

    ```bash
    ls
    ```

    Output (example):

    ```
    -file00  -file01  -file02  -file03  -file04  -file05  -file06  -file07  -file08  -file09
    ```

4. Use the `file` command to identify which file is human-readable:

    ```bash
    file ./*
    ```

    Sample output:

    ```
    ./-file00: PGP Secret Sub-key -
    ./-file01: data
    ./-file02: data
    ./-file03: data
    ./-file04: data
    ./-file05: data
    ./-file06: data
    ./-file07: ASCII text
    ./-file08: data
    ./-file09: data
    ```

    Here, `-file05` is the only file labeled `ASCII text`, meaning it’s human-readable.

5. Display the content of the readable file:

    ```bash
    cat ./-file07
    ```

    Output:

    ```
    4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
    ```

---

### 🔑 Password for Level 5:
    4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw

