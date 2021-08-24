# SMD3528-Chip
Experiments with the SMD3528 RGB LED chip

Hello!

A month ago I ordered 100 cheap RGB LED chips from china (SMD 3528) and noticed that there aren't any clear guides online written. This is a simple project that can be used to help you with any 3.3V-5V LED chips.


For pictures see here: https://www.instructables.com/RGB-LED-SMD3528-Chip-and-Arduino/

#BOM
5V power supply (arduino)

3 x tactile switches

3 x 220ohm resistors various lengths of wire

1 x SMD3528 LED chip

soldering iron (for LEDs without pins)

#Steps
##Step 1: Inspect LED Chip
For this project I am using the SMD3528 chip with no pins, therefore the first step will be to solder some on. If your LED has pins than all you need to do is find the datasheet, or determine polarity. If you have a diode setting on your multi-meter you can use that to test.

![FYMC57EKN6GNE1T](https://user-images.githubusercontent.com/85311146/120693490-ecdf6c80-c45d-11eb-91cd-7a0e3449ca17.png)


If you clip your resistors down like I did you will be left with some metal that we can use. For tiny components I suggest using a handy hands or some similar workbench setup.

##Step 2: Wiring
You will need a basic 5V power supply, hopefully you have an Arduino, you can always tear apart a USB (not recommended)

Most low power LEDs have a max current of approx 25mA, so the Arduino's max 200mA will fry your chip. Therefore we need some current limiting resistors. Check your datasheet for your model but this should be safe more most LEDs

If we do basic OHMS Law, R= V/I = 200

IF YOU DO NOT USE RESISTORS YOU WILL DESTROY YOUR LEDs

Next you need to figure out the polarity on the switches, there are many kinds but a multi meter can tell you if pins are connected before and after button presses.


##Step 3: Power Up and Test
Plug in your Arduino and test. Press the buttons and you can have yourself a light-show! and no programming to boot! Test our different combinations to get new colours.

If it lights up and goes dim, you've burnt it out. If it doesn't light up test your switch or check the polarity on the LED chip.
