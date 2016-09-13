# Arduino-Game-Timer
## Version 1.1
## Authors Chase Cooley, Joey Meyer

A project Chase Cooley and myself worked on to help add complexity to Airsoft matches. You should be able to replicate this project by following our Instructable at http://www.instructables.com/id/Prop-bomb/

#Project Outline
My friend and i built this prop for airsoft/paintball matches.  Its sort of like capture the flag only disarm the "bomb".
How it works is there is a predetermined time limit (which u can change in the code) and the opposing team has that much time to find the code and the bomb and disarm it.  How they find the code is up to you... capture a person? sure!  Find it hidden somewhere? sure! or whatever!  When the bomb is turned on it asks for a code and you can enter in any four number combo and that is the disarm code for that round.  If the person puts in the wrong code it will add 1min 30sec to the time when the time runs out? BOOM! well thats what it says on the screen and it makes a funky noise = ]  This is version 1.0 hopefully in the future we will add wires to unplug to disarm it and some other neat things but for now this is perfect and works well for what we want!  I hope you enjoy the instructable!

#Step One: Aquiring your components
### Electron Components
* 1 Arduino                          (We use duemilanove and you can buy these everywhere online)
* 1 Arduino Proto-Shield  (or if you want just a breadboard or protoboard)
* 1 LCD Screen 16x2       ( we used this one from sparkfun! http://www.sparkfun.com/products/255)
* 1 Numeric KeyPad        ( we used another one from sparkfun! http://www.sparkfun.com/products/8653)
* 1 Potentiometer             ( we used a 50k i believe! bought from raidoshack awhile ago)
* 1 8Ohm Speaker           ( tore one out of an old toy, but you can find them EVERYWHERE!)
* 1 Green LED 
* 1 Red LED
* 4 1k Ohm resistors

### Other Materials:
* Some sort of case ( we found ours at a thrift store but i think they sell them at walmart)
* a chunk of wood   ( this is to bring the arduino off of the bottom of the case and up towards the top)
* Screws                    (to attach the arduino to the chunk of wood)
* Heat shrink tubing

### Tools
* Soldering Iron
* Solder
* Wire     (we used alot of old computer cable so it would stay kinda together)
* Wire Cutters
* Hot Glue Gun
* Hot Glue
* Saw
* Dremel
* Screw driver

#Step Two: Customizing your box
![Arduino Placement](https://cdn.instructables.com/FC1/ZLW8/GLL4ZND0/FC1ZLW8GLL4ZND0.MEDIUM.jpg)
This is basically up to you how you want the layout to be ... you could have everything inside so when u open it up u can see all of the nice hardware and it looks more low budget (as if this isn't low budget enough!) or you can make it clean where you only see the keypad and such.... anyways its all up to you its really just a style thing.
We cut the square out for the lcd screen and then drilled the holes for the LEDS, then cut out the keypad and we just eyed everything as far as positioning. We did all our cutting with a dremel and razor blade.

We then cut the slots in the back:  First we cut a hole for the potentiometer to fit through, then we cut another hole in the back just for the power adapter hole and then also a hole for the USB cable just for programming if we needed to we wouldn't have to take the arduino out.
all of these holes and such are your call for style so just do a layout of everything until you get it how you like it then make the cuts.


#Step Three: Securing your arduino
![Arduino Placement](https://cdn.instructables.com/FKP/03AK/GLL4ZNCQ/FKP03AKGLL4ZNCQ.MEDIUM.jpg)
For our case we raised the Arduino off the case. We used a small block of wood to achieve this. We glued the wood down to the case and 
screwed the Arduino into the wood. You may notice the wires sag in the photo above. This is to prevent breaking connections between the different 
hardware components. We recommend giving a bit extra wire in your project as well. 

#Step Four: Wiring your hardware
![Schematic](https://cdn.instructables.com/FQW/1K4B/GLL4ZNCO/FQW1K4BGLL4ZNCO.MEDIUM.jpg)
![Hardware Exposed](https://cdn.instructables.com/FO8/2Y8X/GLL4ZNCP/FO82Y8XGLL4ZNCP.MEDIUM.jpg)
Unfortunately we didn't make a step by step guide for assembling the arduino, but you can try to follow the schematic and outline. Feel free to ask any questions, Chase or I will try to get in touch as soon as possible.

### Arduino Pins:
* DPin 0 = Nothing
* DPin 1 = Nothing
* DPin 2 = Pin 8 on keypad
* DPin 3 = Red LED
* DPin 4 = Green LED
* DPin 5 = Nothing
* DPin 6 = Nothing
* DPin 7 = Pin 4 LCD
* DPin 8 = Pin 6 LCD
* DPin 9 = Speaker +
* DPin 10 = Pin 11 LCD
* DPin 11 = Pin 12 LCD
* DPin 12 = Pin 13 LCD
* DPin 13 = Pin 14 LCD
* APin 0 = Pin 2 Keypad
* APin 1 = Resistor to Pin 3 Keypad
* APin 2 = Pin 4 Keypad
* APin 3 = Resistor to Pin 5 Keypad
* APin 4 = Resistor to Pin 6 Keypad
* APin 5 = Resistor to Pin 7 Keypad

### LCD SCREEN PINS:
* LCD pin1 = Potentiometer 5v 
* LCD pin 2 = Potentiometer GND 
* LCD pin 3 = Potentiometer Middle 
* LCD pin 5 = GND 
* LCD pin 15 = 5v 
* LCD pin 16 = GND

#Step Five: Uploading the code to your Arduino
You can find the code here within this repository. Feel free to alter it in any way nessacary.

#Step Six: Testing!
