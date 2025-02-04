![GitHub All Releases](https://img.shields.io/github/downloads/xrust83/homekit_wifi_thermostat/total)
![GitHub Releases](https://img.shields.io/github/downloads/xrust83/homekit_wifi_thermostat/latest/total)

# HomeKit_Thermostat

Thermostat accessory for remote control of central heating.
You will also need the Eve app to update the firmware, enable settings after a power outage.

It uses DS18B20 to measure temperature and sets current_heating_cooling_status based on other accessory settings.

For example, when the thermostat sets current_heating_cooling_status to heating/off, use EVE to activate the switch accessory.
on/off respectively. You can also set timer based events in Eve to control the target_heating_cooling_status, in others
words, you can create a program when you want to turn the heating on or off.

Now updated to include a screen (SH1106 OLED) and buttons to adjust the target temperature up and down.

The screen will light up during the initial setup and when the power is turned on. And then it will go out after about 10 seconds, it will light up when you press the up or down button, and then go out again about 10 seconds after the last button press. Also, the screen will light up when switching between statuses in the process of work.

GPIO used are as follows:- 

  4 - DS18B20

  12 - Temperature Up (button connect to ground)

  0 - Temperature Down (button conected to ground) 
  
  15 - Heater Relay Pin
  
  13 - Cooler Relay Pin
  
  10 - Set Button (switch connected to ground) 
  
  2 - LED 
  
  14 - SH1106 SCK_PIN
  
  5 - SH1106 SDA_PIN
  
  
  Online XBM redactor. https://xbm.jazzychad.net
