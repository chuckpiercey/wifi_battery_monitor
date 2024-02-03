# wifi_battery_monitor

# Background 

FOLPA recently converted our entire set of Festival of Lights parade floats to LiFePO4 batteries from gas generators (see Board Float Batterization Presentation). The key issue with this change is being sure each float has adequate charge for the complete show (see float batteries plan).

# Project Definition Document: Parade Float Remote Battery Monitoring System

# Summary  
Create small, low power sensors that measure battery voltage (and, potentially, other float characteristics of interest) and report back to a central server that will create a real time dashboard of battery charge levels. This will allow us to remotely monitor floats during the off-season, and the critical pre-parade staging in the parking lot (as well as other uses).

Design the whole solution in a manner that allows for simple extension to additional sensors that might have nothing to do with battery charge levels. Ideally use Lora for communications.

# Baseline Goal
Install a Raspberry Pi data collection and reporting server on the Steam Train float and place ESP32 reporting devices on each float directly connected to the batteries for that float. Report battery charge levels to the PiServer. Ideally, battery charge reporting dashboards could be accessed using a mobile phone.

# Stretch Goal1
Enable the sensors to respond to a Pi-server command for a particular float to power on or off.

# Stretch Goal2
Add a GPS sensor that can (phase 1) track and report float position and speed to a log file, and (phase 2) eventually report speed to a LCD screen that displays the walking speed to float pushers in real time.

