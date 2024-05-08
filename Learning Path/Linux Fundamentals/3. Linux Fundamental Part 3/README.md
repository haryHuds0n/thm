## Linux Fundamental Part 3

<p align="center">
  <img title="portainer" src='https://www.thedutchhacker.com/wp-content/uploads/2021/09/Linux-Fundamentals-Part-3-tryhackme.png' width=700 />
</p>


### Task 3 Terminal Text Editors

1. **Edit `task3` located in `tryhackme's` home directory using Nano. What is the flag?**
    
    ```
    THM{TEXT_EDITORS}
    ```

### Task 4 General/Useful Utilities

1. **Download the file http://MACHINE_IP:8000/.flag.txt onto the TryHackMe AttackBox. Remember, you will need to do this in a new terminal. What are the contents?**
    
    ```
    THM{WGET_WEBSERVER}
    ```

### Task 5 Processes 101

1. **If we were to launch a process where the previous ID was "300", what would the ID of this new process be?**
    
    ```
    301
    ```

2. **If we wanted to cleanly kill a process, what signal would we send it?**
    
    ```
    SIGTERM
    ```

3. **Locate the process that is running on the deployed instance (MACHINE_IP). **What flag is given?**
    
    ```
    THM{PROCESSES}
    ```

4. **What command would we use to stop the service "myservice"?**
    
    ```
    systemctl stop myservice
    ```

5. **What command would we use to start the same service on the boot-up of the system?**
    
    ```
    systemctl enable myservice
    ```

6. **What command would we use to bring a previously backgrounded process back to the foreground?**
    
    ```
    fg
    ```

### Task 6 Maintaining Your System: Automation

1. **When will the crontab on the deployed instance (MACHINE_IP) run?**
    
    ```
    @reboot
    ```

### Task 8 Maintaining Your System: Logs

1. **What is the IP address of the user who visited the site?**
    
    ```
    10.9.232.111
    ```

2. **What file did they access?**
    
    ```
    catsanddogs.jpg
    ```
