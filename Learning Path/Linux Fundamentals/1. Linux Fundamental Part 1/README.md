## Linux Fundametal Part 1

<p align="center">
  <img title="portainer" src='https://www.thedutchhacker.com/wp-content/uploads/2021/09/Linux-Fundamentals-Part-1.png' width=700 />
</p>

### Task 2 A bit of Background on Linux

1. **Research: What year was the first release of a Linux operating system?**
    ```
    1991
    ```

### Task 4 Running Your First New Commands

1. **If we wanted to output the text "TryHackMe", what would our command be?**
    ```
    echo TryHackMe
    ```

2. **What is the username of who you're logged in as on your deployed Linux machine?**
    ```
    tryhackme
    ```

### Task 5 Interacting With The Filesystem!

1. **On the Linux machine that you deploy, how many folders are there?**
    ```
    4
    ```

2. **Which directory contains a file? **
    ```
    folder4
    ```

3. **What is the contents of this file?**
    ```
    Hello World!
    ```

4. **Use the cd command to navigate to this file and find out the new current working directory. **What is the path?**
    ```
    /home/tryhackme/folder4
    ```

### Task 6 Searching for Files

1. **Use grep on "access.l**og" to find the flag that has a prefix of "THM". **What is the flag?**
    ```
    THM{ACCESS}
    ```

2. **And I still haven't found what I'm looking for!**
    ```
    No Answer Needed
    ```

### Task 7 An Introduction to Shell Operators

1. **If we wanted to run a command in the background, what operator would we want to use?**
    ```
    &
    ```

2. **If I wanted to replace the contents of a file named "passwords" with the word "password123", what would my command be?**
    ```
    echo password123 >> passwords
    ```

3. **Now if I wanted to add "tryhackme" to this file named "passwords" but also keep "passwords123", what would my command be**
    ```
    echo tryhackme >> passwords
    ```

4. **Now use the deployed Linux machine to put these into practice**
    ```
    No Answer Needed
    ```