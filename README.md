# wifi_battery_monitor

# Background 

To fight climate change [(See FOLPA and Climate Change)](https://docs.google.com/presentation/d/1xozE2pJLaS6ZU5rT9S0h937FgYKbp3cBDq__n-NryBE/edit#slide=id.g243b82910f1_0_0), FOLPA recently converted its entire set of Festival of Lights parade floats to LiFePO4 batteries from gas generators (see [Board Float Batterization Presentation](https://docs.google.com/presentation/d/1xozE2pJLaS6ZU5rT9S0h937FgYKbp3cBDq__n-NryBE/edit#slide=id.g243b82910f1_0_0)). The key issue with this change is being sure each float has adequate charge for the complete show (reference [float batteries plan](https://docs.google.com/spreadsheets/d/1jNfh3eLkbha0XVxC8WWYtK-C9kAY6Rwcxe5QWCYV6Zo/edit#gid=0)).

# Project Definition Document: Parade Float Remote Battery Monitoring System

The goal of this project is to automatically track and report battery storage levels (and other data points of possible interest like GPS location, speed and CO2 levels).

# Summary  
Create small, low power sensors that measure battery voltage (and, potentially, other float characteristics of interest) and report back to a central server that will create a real time dashboard of battery charge levels. This will allow us to remotely monitor floats during the off-season, and the critical pre-parade staging in the parking lot (as well as other uses).

Design the whole solution in a manner that allows for simple extension to additional sensors that might have nothing to do with battery charge levels. Ideally use Lora for communications.

# Baseline Goal
Install a Raspberry Pi data collection and reporting server on the Steam Train float and place ESP32 reporting devices on each float directly connected to the batteries for that float. Report battery charge levels to the PiServer. Ideally, battery charge reporting dashboards could be accessed using a mobile phone.

# Stretch Goal1
Enable the sensors to respond to a Pi-server command for a particular float to power on or off.

# Stretch Goal2
Add a GPS sensor that can (phase 1) track and report float position and speed to a log file, and (phase 2) eventually report speed to a LCD screen that displays the walking speed to float pushers in real time.

