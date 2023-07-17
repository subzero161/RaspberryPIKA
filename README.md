# RaspberryPIKA
This project uses Raspberry Pi and Kali to build a portable and usable handheld device.
I have always wanted a handheld Raspberry Pi. Most of the videos I found online did not have instructions or proper guidance.
I am focusing on the attainability and usability of the product, not just something that will sit in the back of my storage box.
I will link to the products that I am using and my justifications for choosing said products. 
If you are following this project, use it as a guide to modify the product to your needs.
I have a lot of the things lying around that I am using and I will also put links to other products I would want to use if I did not have it lying around.
I have always wanted a mini but functional keyboard for the vision of building something like this for years. I would like to give a shout-out to "arturo182" and "solderparty" for making a useful and functional keyboard.
Here is a list of all the products I am using.
## Raspberry PI
Raspberry Pi Model 4B 8GB -$74.99
https://www.microcenter.com/product/622539/raspberry-pi-4-model-b-8gb-ddr4
I was lucky enough to get it at my local Microcenter in-person. I understand this is not an ideal situation for everyone, but please do not pay scalpers as I have taken over 6 months to slowly gather everything I am using for this unless you need it for work and it is urgent or will make a significant quality of life improvement even if you overpay for it.
## MicroSD
MicroSD: I am using an old 32GB Sandisk MicroSD lying around, but feel free to use any card with a minimum of 32GB or more. As of writing this, I am ordering a Samsung 128GV microSD on sale for $9.99. Again, you do not need a card unless you have a specific need for storage.  I know that I might need to use it as a SQL server occasionally for my school projects and don't want to switch cards all the time.
https://www.samsung.com/us/computing/memory-storage/memory-cards/evo-select-adapter-microsdxc-64gb-mb-me64ka-am/
https://a.co/d/dxx30yz
## Keyboard
Now for the star of this show, it is this keyboard, made using an RP2040 and a Blackberry Q20 keyboard with an optical trackpad.
Honestly, I have always wanted a similar product to this but never knew where to start.
The optical trackpad is really helpful for me.
https://www.tindie.com/products/arturo182/bb-q20-keyboard-with-trackpad-usbi2cpmod/
## Display
The next item on my list was a Display, I am using an older display I had lying around that I never got to using for my 3D Printer. It uses DSI interface and is 5 inches. I wanted a display that was readable and usable. Feel free to use any display you have lying around. 
I am using V1.0 of the BigTreeTech PiTFT 50, but V2.0 has a dial to control the brightness. MSRP $55.99
https://a.co/d/6j7Bko6
## Battery
This is something I had to put some thought into, I wanted a battery that would be able to provide at least 15W of power to the Raspberry PI.
I wanted something that was small and not bulky, with an option to charge from the side and a way to show how much battery is left on the Power Bank.
The display should show the percentage, not just an LED light indicator.
The second priority was at least 10000mAh.
Charmast 10000mAh 
Color: A-black-S
https://a.co/d/7jbVRtt
I have paid $22.99 and would not an any more than that on a battery for this project.
Feel free to use any you have lying around.
## Cables
I am using the USB A to USB C cable that comes with the battery. As far as the cable for the keyboard, I had one lying around that met my needs but it was bulky.
I wanted an angled type C connector so it took less space on the battery, but it is a bulky cable. I have looked on Amazon for alternate products and so far have come up with this:
https://a.co/d/cbcase9
MSRP $6.98, price fluctuates, keep an eye out
## Fan/Heatsink
I am using a heatsink and fan from some other projects and do not have the proper information, but I think this would make a great alternate product:
https://www.waveshare.com/product/raspberry-pi/accessories/pi-fan-3007.htm
## Miscellaneous Items that you will need
### Heavy-duty double-sided tape. 
I had some lying around from other things around the house but I am using this one.
https://www.homedepot.com/p/Scotch-1-in-x-11-1-yds-Permanent-Double-Sided-Extreme-Mounting-Tape-414-LONGDC/205507375
https://a.co/d/e8iKDo5
### Velcro
I am also using Velcro to attach the keyboard since I want to use the keyboard on other projects simultaneously.
https://a.co/d/hCOx3E4
You can also use the double-sided tape if you don't plan on using the keyboard again.
### M2.5 thread screw and stand-off set
You do not need this item, but I am able to integrate the battery better into the system by increasing the height with the stand-offs.
https://www.adafruit.com/product/3299
https://thepihut.com/products/adafruit-black-nylon-screw-and-stand-off-set-m2-5-thread

### Bunch of Type-C connectors
It will make your life easier by connecting/disconnecting from the battery and also having an open connection for type-c input/output from the battery.
Feel free to get any other products as long as you have a U-shaped connector.
https://a.co/d/04ecHyK

## Operating System
Kali Linux for ARM
Download the latest 64-bit version
Kali for Raspberry PI has native support for DSI displays.
https://www.kali.org/get-kali/#kali-arm

## Step 1
### Setting up the Raspberry PI
#### Head to this webpage and download Raspberry Pi Imager
https://www.raspberrypi.com/software/
Follow instructions on how to install any OS
#### Head to Kali website
https://www.kali.org/get-kali/#kali-arm
Select 64-bit for Raspberry Pi and download
#### Follow installation instructions on how to install a custom OS
You can also choose to use Other OS from Raspberry Pi imager and select Kali
### Issues
After I fully upgraded the OS using "sudo upgrade", the device exits out of the GUI, I would recommend waiting for a bit until there are solutions available. So far I have not been able to find a solid answer, so probably best to hold off on the upgrade unless you upgrade individual packages.

## Step 2 
### Assemble display, Raspberry Pi and Heatsink/Fan
