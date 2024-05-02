## Web Application Security

### Learn about web applications and explore some of their common security issues

<img src="f054e83e6b7c61f643222f8141105daf.png" alt="drawing" width="800"/>

### Task 1 Introduction To Digital Forensics

1. **Consider the desk in the photo above. In addition to the smartphone, camera, and SD cards, what would be interesting for digital forensics?**

    ```
    laptop
    ```

## Task 2 Digital Forensics Process

1. **It is essential to keep track of who is handling it at any point in time to ensure that evidence is admissible in the court of law. What is the name of the documentation that would help establish that?**

    ```
    Chain of custody
    ```

## Task 3 Practical Example of Digital Forensics

1. **Using `exiftool` or any similar tool, try to find where the kidnappers took the image they attached to their document. What is the name of the street?**
  
    We can use `exiftool` to look into metadata of image and found GPS Location Data, after convert it to correct format, paste it in [google map](https://map.google.com) and we can find out what street it is

    ```
    Milk Street
    ```

2. **What is the model name of the camera used to take this photo?**

    For the model of the camera, we can look closer to the metadata of the image but we have an easy way to find it using [grep](https://man7.org/linux/man-pages/man1/grep.1.html), we can use this command to get the model of the camera

    ```bash
    exiftool IMAGE.jpg | grep model
    ```

    What is the model name of the camera used to take this photo?
    ```
    Canon EOS R6
    ```
    