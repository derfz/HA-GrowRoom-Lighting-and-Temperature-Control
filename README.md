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
daytime and nightime (lights on/off) temp can be inmdividually set so you can choose the difference. I've set mine to 2 degrees.  

## Helpers


## Templates


## Installation
