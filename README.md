# InternetofThings
Homework for IoT

For the homework for thursday 14 october we needed to write a manual about controlling a LEDstrip through Telegram.
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

So I tried that aswell, and it worked.


So what I did was follow all the steps from the site, and i switched HIGH to LOW and visa versa.

After that I started trying to get the ledstrip to work.
After searching on google for a long time I found this manual that looked promising:
https://www.instructables.com/IoT-Manual-Digital-Remote-for-LED/

At some point it said to install the library: esp8266 by ESP8266 Community (version 2.5.0)
I didn't find it in the library manager and I couldn't find it on the internet, so that also didn't work.  
It also said to open LEDCONTROL in Arduino. Couldn't find that file anywhere aswell.

Next I went to this page:
https://github.com/witnessmenow/Simple-Home-Automation-With-Telegram

There I found LEDCONTROL. Then I went back to the manual I found earlier in the day.
Also didn't work.

Then I tried the manual again. It contained a video which shows how they build the manual, so i tried it with the video:
https://www.youtube.com/watch?v=-IC-Z78aTOs&t=24s

In the end I couldn't manage to make it work.

These are the sites I visited:
https://iotdesignpro.com/projects/telegram-controlled-home-automation-using-esp8266
https://www.youtube.com/watch?v=-IC-Z78aTOs
https://www.reddit.com/r/arduino/comments/auehwu/controlling_led_lights_with_an_esp8266_using/
https://arduinodiy.wordpress.com/2020/01/06/3838/
https://github.com/topics/esp8266-projects?l=c%2B%2B&o=asc&s=updated
https://github.com/thebigpotatoe/Super-Simple-RGB-WiFi-Lamp
https://github.com/eighthree/Simple-LED-Strip-Controller
https://github.com/witnessmenow/Universal-Arduino-Telegram-Bot
https://www.makeuseof.com/tag/connect-led-light-strips-arduino/
https://www.huizebruin.nl/arduino/esp_8266-8566/tutorial-schakelen-van-esp8266-via-telegram-bot/
