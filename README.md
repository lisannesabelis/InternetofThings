# InternetofThings
Homework for IoT

For the homework for thursday 14 october we needed to manage a LEDstrip through Telegram.
This document will show how the process of managing that went.

I found a site on google that showed how to make it work:
This is only the part about making the led on the board work.
https://randomnerdtutorials.com/telegram-control-esp32-esp8266-nodemcu-outputs/
I followed the steps in the document, but it didn't work right away.

The bot was connected and everything said it worked.
The serial monitor showed that aswell:
![image](https://user-images.githubusercontent.com/74072161/137131133-5bbeaf8a-cb77-4aa7-906b-f6cba95ca84e.png)

The only problem was that the LEDstrip itself would'nt turn off.
I found something on the site that said that when you're using the ESP8266, the LED works with inverted logic. So I decided to try that, since I didn't do that.
![image](https://user-images.githubusercontent.com/74072161/137131559-5dbe2a6c-26b9-42cd-bf9f-9ae546917878.png)

I changed it, but it still didn't work.
Then it said that this needs to be done:
![image](https://user-images.githubusercontent.com/74072161/137132345-a57b285c-03aa-4b8f-b605-beaf721de525.png)

So I tried that aswell, and it worked!

So what I did was follow all the steps from the site, and i switched HIGH to LOW and visa versa.

After that I started trying to get the ledstrip to work.
I've googled for 2 hours and I still couldn't find anything.
Then I found this manual:
https://www.instructables.com/IoT-Manual-Digital-Remote-for-LED/

At some point it said to install the library: esp8266 by ESP8266 Community (version 2.5.0)
I didn't find it in the library manager, so that didn't work aswell. 
It also said to open LEDCONTROL in Arduino. Couldn't find that file anywhere aswell.

Next I went to this page:
https://github.com/witnessmenow/Simple-Home-Automation-With-Telegram

There I found LEDCONTROL. Then I went back to the manual I found earlier in the day.
