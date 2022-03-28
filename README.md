# adGuardMonitor
Uses Blinkt library on a RaspberryPi to Display AdGuard Home Status and Add Percentage

You will require to have your AdGuard Home Instance on a seprate RaspberryPi than the device this runs on  

# Auto Start Script
sudo nano /etc/rc.local  
Add the the location the script will run from to the end of the file    
i.e "python3 /home/username/projects/adGuardMonitor/main.py &"  
ensure the file ends with "exit 0"  


# Features
Blinkt features 8 super bright RGB LEDs that neatly fit onto your RaspberryPi's GPIO  
AD blocked percentage is displayed as GREEN LEDs filling up the BLINKT module  
If no connection to your AdGuard Home instance is detected - LEDs will radiate in RED  

If AdGuard Home is disabled the LEDS will cycle through through colours running up and down the Module

Lights switch off at: 22:00  
Lights Switch on at: 08:00 

# Requirements
Download [blinkt](https://github.com/pimoroni/blinkt) python Library
AdGuard [Python Client](https://pypi.org/project/adguardhome/)

# TODO
Implementation
