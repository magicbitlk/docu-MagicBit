================
Beginners Guide to Magic Bit
================
In this guide we are learning how to use the basic components on the Magic Bit board. The components comes with the Magic Bit is arranged as following. We have provided code examples as well as self assignment set to enhance your knowledge.   

.. image:: https://github.com/magicbitlk/Magicbit-Arduino/raw/master/Resources/Layout.png


*************************
Example 1: Blinking an LED
*************************
Introduction
************
     In this example you are learning how to turn on and off a LED or any other actuator which can be controlled by a digital output such as relay, bulb, motor.

Learning Outcomes
*****************
 From this example, you'll get an understanding about,
-  Pin Mode
-  Digital Write
-  Delay Functions

Components
**********
- Magic Bit

Theory
**********
 A digital output allows you to control a voltage with an electronic device. If the device instructs the output to be high, the output will produce a voltage (generally about 5 or 3.3 volts). If the device instructs the output to be low, it is connected to ground and produces no voltage.Here magicbit is the device and output voltage is either 3.3V for HIGH and 0V for LOW.

Methodology
***********
 Magicbit equipped with four onboard leds in magicbit development board, Lets select yellow LED (which is wired to D18)

 .. image:: https://github.com/Ruwatech/docu-MagicBit/blob/master/Resources/image4.png?raw=true
 By setting output state to high of LED pin will turn on the led and by setting output state to LOW will turn of LED.

Coding
******
 .. code-block:: c

     void setup(){
	pinMode(18,OUTPUT);
     }
     void loop(){
	digitalWrite(18,HIGH);
	delay(1000);
	digitalWrite(18,LOW);
	delay(1000);
     }


