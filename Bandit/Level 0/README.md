# OverTheWire: Bandit Wargame Walkthrough

This repository contains a level-by-level walkthrough of the **Bandit** wargame from [OverTheWire](https://overthewire.org/wargames/bandit/), aimed at helping beginners understand Linux basics, file system navigation, and shell commands.

---

## 📘 Bandit Level 0

### 🧩 Level Goal

> The goal of this level is for you to log into the game using SSH.

**Host:** `bandit.labs.overthewire.org`  
**Port:** `2220`  
**Username:** `bandit0`  
**Password:** `bandit0`

---

### 🛠 Tools Used

- Linux Terminal 
- SSH Protocol

---

### 🪜 Steps to Solve

1. Open your terminal and type the following command to log into the remote server using SSH:

    ```bash
    ssh bandit0@bandit.labs.overthewire.org -p 2220
    ```

2. When prompted, enter the password:

    ```
    bandit0
    ```

3. Once logged in successfully, you’ll see a welcome message and the terminal prompt will change to something like:

    ```
    bandit0@bandit:~$
    ```
