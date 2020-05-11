# Airway-Ventilation
Prototype for Emergency Airway Ventilation Training Device

# Hardware Assembly Guide

#### STEP 1: Set up a breadboard with Arduino
![](./img/arduino.jpeg)
The red rail is connected to the +5V pin of the Metro Mini, and the blue rail is connected to the GND pin.

#### STEP 2: Connect the flex sensor
![](./img/flex.jpeg)
One pin of the flex sensor is connected to the A0 pin, and the other to +5V (the red rail). Add a resistor in between. 

#### STEP 3: Hook the graphic display
![](./img/display.jpeg)
Now let's connect the OLED display. Hook:

* GND to ground (the blue rail)
* VCC to +5V (the red rail)
* SDA to A4
* SCL to A5

#### STEP 4: Plug in the circuits
![](./img/full1.jpeg)
Connect the Arduino to your computer using the USB cable. And stick the sensor to the balloon (or whatever you are measuring).

![](./img/full2.jpeg)

Now you have finished connecting the circuits and can turn to the below Software Assembly Guide to upload code to your Arduino. It should be ready to go!


# Hardware Cost 

The components can be ordered online from any place like Adafruit, Mouse, DigiKey, Amazon, etc. The estimate total price is ~$35,
which is broken down as follows:

Metro Mini ~$12 

Flex sensor ~$8 

Display ~$5

Breadboard ~$3

Jumper wires ~$1

Balloons ~$2 

Tube ~$2

USB cable ~$2

Resistors ~$0.30


# Software Assembly Guide

The first step is to download the Arduino IDE, which can be found on https://www.arduino.cc/en/main/software

Once you have downloaded and installed the Arduino IDE, you should see a screen like the one below. 

![](init_arduino_pic.png)

Download the flex_sensor_code folder from this repository and open it using the Arduino IDE by clicking on File -> Open... and selecting the folder. Once the sketch is loaded, your screen should look like this:

![](loaded_arduino_pic.png)

You should install two extra libraries to run the code. The first one can be found by going to `Tools > Manage Libraries > Search Adafruit GFX Library`. The second one can be found by `Tools > Manage Libraries > Search Adafruit SSD 1306`.

Connect the Arduino to the computer using a USB cable. Make sure the right Board and Port options are selected by clicking on Tools. Next, 
click on Upload and wait for the code to be uploaded to the Arduino. 

You're all set now, great job!
