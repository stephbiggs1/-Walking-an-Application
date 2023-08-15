# Walking-an-Application

Room Link: https://tryhackme.com/room/walkinganapplication#

Overview: Manually review a web application for security issues using only your browsers developer tools. Hacking with just your browser, no tools or scripts.

---

Tools used: 

- THM Virtual Machine
- Browser Developer tools

  
![website](https://github.com/stephbiggs1/-Walking-an-Application/assets/62307870/d9937c42-c363-4f75-beb5-d6112489bf5f)

## Viewing Page source

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6dcd8a68-94ba-4324-8a44-9c5327782237/Untitled.png)

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/7d749c89-6dcc-4e85-ad48-758f10ad3a05/Untitled.png)

  Flag 1: found in HTML comment one via /new-home-beta

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/4645359c-7aff-428c-b02e-2dc0372b392d/Untitled.png)

Flag 2: Found in embedded secret link on line 41 of page source

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/cba918fc-4999-4064-934a-7bfe46d82d60/Untitled.png)

Fla 3: Found via /assets/ in flag.txt folder

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/dcef083a-81ef-4542-b562-43b0c56abe8d/Untitled.png)

Flag 4: Found by navigating to site in HTML comment on line 51. I navigated to the change log page and read information for current version 1.3. I navigated to file /tmp.zip, downloaded folder and located flag found within the folder. 

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a4d72907-1f32-495b-aacc-936a177408af/Untitled.png)

## Inspector Tools

Flag 1: opened inspector tool in chrome browser and navigated to the paywall. Under elements and style I was able to edit the display from block to none and was able to see corresponding flag.

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/63dda87d-1c0f-4e7d-8b83-17915e53b0e8/Untitled.png)

## Debugger

Flag 1: In order to pause the flash animation, I navigate to the sources page and clicked text beside second to last line. 

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/ed5d3069-9971-4288-a87a-7cc91e0e9d5d/Untitled.png)

## Network

Flag 1: Under the network tab I was able to keep track of incoming messages from the contact page. One a message was submitted I was able to click on newly generated information and discover the flag within the message preview.
