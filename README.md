jurek_control
=============

Raspberry pi driver for Tortoise/terrarium automation 

This is a 0.1a version of my project to automate the tortoise terrarium at home.

At the moment there is only one water-pump connected to the Pi that sprinkles water every hour to sustain humidity.

I plan to add an autmatic feeder and "weather station" for monitoring humidity and temperature.

    Usage:
      jurek_control heater (--turn-on <minutes> | --turn-off | --status)
      jurek_control pump (--turn-on <seconds> | --turn-off | --status)
      jurek_control feeder (--turn-on <seconds> | --turn-off | --status)
      jurek_control status
      jurek_control (-h | --help)
      jurek_control (--version)
      

Example usage:
      
```shell
root@raspberrypi:/home/pi# jurek_control status
 Pump is turned off
 Electric heater is turned off
 Feeder is turned off

root@raspberrypi:/home/pi# jurek_control pump --turn-on 10  # in seconds
 2013-11-19 14:26:12.468362 Turning pump on
 2013-11-19 14:26:22.474739 Turning pump off

root@raspberrypi:/home/pi# jurek_control heater --turn-on 1  # in minutes
 2013-11-19 14:27:14.478262 Turning heater on
 2013-11-19 14:28:14.484139 Turning heater off
```
