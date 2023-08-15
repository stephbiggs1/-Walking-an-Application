# Walking-an-Application

Room Link: https://tryhackme.com/room/walkinganapplication#

Overview: Manually review a web application for security issues using only your browsers developer tools. Hacking with just your browser, no tools or scripts.

---

Tools used: 

- THM Virtual Machine
- Browser Developer tools

  
![website](https://github.com/stephbiggs1/-Walking-an-Application/assets/62307870/d9937c42-c363-4f75-beb5-d6112489bf5f)

![source](https://github.com/stephbiggs1/-Walking-an-Application/assets/62307870/d49e11d0-5923-4b7e-992b-fe4206a9ec63)


## Viewing Page source

  Flag 1: found in HTML comment one via /new-home-beta

![flag 1](https://github.com/stephbiggs1/-Walking-an-Application/assets/62307870/fc029789-a85b-4fa5-a304-3d4cfa6dcbba)


Flag 2: Found in embedded secret link on line 41 of page source

![flag 2](https://github.com/stephbiggs1/-Walking-an-Application/assets/62307870/43eb235b-fdda-433d-bfd8-f8b8e99fee17)

Fla 3: Found via /assets/ in flag.txt folder

![flag 3](https://github.com/stephbiggs1/-Walking-an-Application/assets/62307870/decd50de-ca15-4303-9cf9-77ac5310a386)


Flag 4: Found by navigating to site in HTML comment on line 51. I navigated to the change log page and read information for current version 1.3. I navigated to file /tmp.zip, downloaded folder and located flag found within the folder. 

![flag4](https://github.com/stephbiggs1/-Walking-an-Application/assets/62307870/a1d175d9-133e-4345-90d4-e696ed92f145)

## Inspector Tools

Flag 1: opened inspector tool in chrome browser and navigated to the paywall. Under elements and style I was able to edit the display from block to none and was able to see corresponding flag.


![flag5](https://github.com/stephbiggs1/-Walking-an-Application/assets/62307870/581b2672-0836-4e2f-9ebe-f174e0f6b002)


## Debugger

Flag 1: In order to pause the flash animation, I navigate to the sources page and clicked text beside second to last line. 

![flag 6](https://github.com/stephbiggs1/-Walking-an-Application/assets/62307870/5b70ae58-a6a3-4456-99b7-d00f53a22c36)

## Network

Flag 1: Under the network tab I was able to keep track of incoming messages from the contact page. One a message was submitted I was able to click on newly generated information and discover the flag within the message preview.

![flag 7](https://github.com/stephbiggs1/-Walking-an-Application/assets/62307870/cf6c4d4a-1f8e-48e7-a790-787f3deaf634)

