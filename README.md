# HA-GrowRoom-Lighting-and-Temperature-Control

## Premis of project
The idea behind this project was to start to fully automate all features of my grow room.  
As I only have lights and heat to control as yet, that is where I have started.  

## caveat
As I am NOT a programmer all code was written with the help of ChatGPT.  

## Lighting Control
Lighting is based on a standard 12 week grow cycle. 4 weeks veg, 8 weeks flower.  
Lighting cycle is 18/6 veg and 12/12 flower.  
The lighting cycle is centered at noon. This means that your 18/6 lighting cycle is 0300-2100 and your 12/12 cycle is 0600-1800. This you have no control over.  

## Heating control
Heating is tied into the lighting in the project.  
This is because the temperature during the day is higher than the temperature at night.  
This closely mimics what plants actually experience naturally.  
Setpoint/Hysteresis is set manually. Sanity checking is included to ensure you don't set any minimum temp above the maximum temp. This will result in the heater switch being dissabled.   
Daytime and Nightime (lights on/off) temp can be inmdividually set so you can choose the difference. I've set mine to 2 degrees.  

## Helpers
###### Grow Start Date
- input_datetime.grow_start_date
###### Daytime high temp
- input_number.grow_day_temperature_high
###### Daytime low temp
- input_number.grow_day_temperature_low
###### Nighttime high temp
- input_number.grow_night_temperature_high
###### Nighttime low temp
- input_number.grow_night_temperature_low
###### Absolute maximum temp your grow rome will get to before the heater is forced off
- input_number.grow_absolute_max_temp
###### Absolute lowest temp your grow groom will get to before the heater is forced on
- input_number.grow_absolute_minimum_temp

## Templates
The templates.yaml whilst not essential contains information about when lights turn on/off, a countdown timer to the next cycle, current grow week and several others that will assist in debugging the system if it doesn't work as expected.  
Don't forget to change your_lights_switch, this has to be done manually.  

## Installation
I will setup quicklink buttons to install everything automatically.   

## Setup
Firstly set the start date of your grow.   
Then set the temperature settings. Ensure you don't set the minimum temp above the maximum temp. The difference between min/max can be 0.1 (this is your setpoint/hysteresis)   
