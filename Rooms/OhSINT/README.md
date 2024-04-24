## OhSINT
### Are you able to use open source intelligence to solve this challenge?


![OhSINT](https://tryhackme-images.s3.amazonaws.com/room-icons/9c6bc7e6db746ea68ecaa99e328923f1.png)


* Difficulty: Easy
* ETC: 60min

### Task 1 OhSINT
What information can you possible get with just one photo?


1. **What is this user's avatar of?**

    Image can contain hidden data so you can you tools like exiftool to extract information about the image
    ```bash
    ExifTool Version Number         : 12.70
    File Name                       : WindowsXP_1551719014755.jpg
    Directory                       : /root
    File Size                       : 234 kB
    File Modification Date/Time     : 2024:04:24 08:45:30+00:00
    File Access Date/Time           : 2024:04:24 08:49:10+00:00
    File Inode Change Date/Time     : 2024:04:24 08:49:14+00:00
    File Permissions                : -rw-r--r--
    File Type                       : JPEG
    File Type Extension             : jpg
    MIME Type                       : image/jpeg
    XMP Toolkit                     : Image::ExifTool 11.27
    GPS Latitude                    : 54 deg 17' 41.27" N
    GPS Longitude                   : 2 deg 15' 1.33" W
    Copyright                       : OWoodflint
    Image Width                     : 1920
    Image Height                    : 1080
    Encoding Process                : Baseline DCT, Huffman coding
    Bits Per Sample                 : 8
    Color Components                : 3
    Y Cb Cr Sub Sampling            : YCbCr4:2:0 (2 2)
    Image Size                      : 1920x1080
    Megapixels                      : 2.1
    GPS Latitude Ref                : North
    GPS Longitude Ref               : West
    GPS Position                    : 54 deg 17' 41.27" N, 2 deg 15' 1.33" W
    ```

    From information extract from exiftool, we notice that the `copyright` field was `OWoodflint` so we tracked down all social media account and we found this X [account](https://twitter.com/OWoodflint) and was able to answer the first flag.

    ```
    cat
    ```
2. **What city is this person in?**

    From the social media account that we found in previous step, we notice that he have a post that contain BSSID `B4:5D:50:AA:86:41`.
    
    FYI, the [BSSID and SSID](https://www.atera.com/blog/computer-terms-unwrapped-what-is-bssid/#:~:text=BSSID%20stands%20for%20Basic%20Service%20Set%20Identifier%2C%20and%20it's%20the,to%20connect%20to%20the%20WiFi.) relate to Wifi Network and there is a website that can track down BSSID and SSID in the world. It is [Wigle.net](https://wigle.net/)

    Enter BSSID to the website and move around the map, you will able to see the city where the Wifi locate

    ```
    London
    ```

3. **What is the SSID of the WAP he connected to?**

    From the previous information, zoom in the map and you will able to see the SSID of the wifi network.
    ```
    UnileverWifi
    ```

4. **What is his personal email address?**

    After searching around the Wigle.net site, we can see is nothing left for us to discover so we when back to google seach engine where we started and found some other website contain the word `OWoodflint`.

    ![Image](https://i.imgur.com/x1CSzQF.png)

    View the github website and we will see the email address maybe belong to `OWoodflint`

    ```
    OWoodflint@gmail.com
    ```

5. **What site did you find his email address on?**

    ```
    github
    ```

6. **Where has he gone on holiday?**

    From the github site above, we notice that the author have a link to his [wordpress](https://oliverwoodflint.wordpress.com/) website

    From the wordpress site, we can answer the question above

    ```
    New York
    ```

7. **What is the person's password?**

    Poking around OWoodflint wordpress site, nothing useful comeup.
    The question is asking for password so we think he maybe hide it some where on website. We open Dev Tool to look in source code and some tab like Application, Network, Memory and guess what, we found something odd in source code so we decide to submit it into question and woola, answer correct

    ![image](https://i.imgur.com/pvs7uk6.png)

    ```
    pennYDr0pper.!
    ```

The rooms is now completed.