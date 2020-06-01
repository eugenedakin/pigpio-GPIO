# pigpio-GPIO
Code for Xojo apps to access the Raspberry Pi GPIO pins through the pigpio library

This is a pigpio library that is a replacement for the deprecated wiringPi library that
is to be used with Xojo apps. A book has been written called 'I Wish I Knew How To...
Program Raspberry Pi 4B Electronics with Xojo: Buster Edition' is being written and the 
examples use this library exclusively. More instructions about the book will be available
at https://www.scispec.ca and press the button on books.

The pigpio library is installed by default on the Raspbian OS (May 2020) and instructions 
are available at http://abyz.me.uk/rpi/pigpio/download.html.

A historic review is that the first Raspberry Pi Electronics book for Xojo was written
with wiringPi in June of 2016. Many examples were added and updated from Raspberry Pi 2B and
Raspberry Pi 3B boards. Major updates to the book occured when Raspberry Pi 3B+ arrived with
the new operating system. 

As of May 2020, the latest Operating System is Raspbian Buster, with Raspberry Pi 4B, 
using Xojo's 2019 R3.1 (Xojo API2) code. 

Original work for the first Raspberry Pi wiringPi code to Xojo library was with Paul Lefebvre 
(https://github.com/paullefebvre). 

Another library was created by Ulrich Bogun (https://gitlab.com/UBogun/Xojo-pigpio)
and has been instrumental with the creation of this library.

With the changes in Raspberry Pi motherboard, Buster Opeating System, Xojo API2, and deprecation
of wiringPi, a new book is being written that provides examples, explanations, and 
data for all of these recent changes. 

The estimated time for the book to be released is the fall of 2020. 

Version 1.0 (18 May 2020)
-Initial Version of pigpio-GPIO library

Version 1.1 (19 May 2020)
-The pigpio class was converted to an object to make the code very similar to 
those examples used in Python. 

v1.2 (20 May 2020)
-Added many error constants (over 150)
-Added gpio_read method
-Added gpioSetPullUpDown method and constants

v1.3 (29 May 2020)
-Added gpioInitialise
-Added hardware_PWM
-Added gpioPWM
-Added gpioSetPWMRange

v1.4 (31 May 2020)
-Added gpioSetPWMFrequency
-Added gpioTerminate
-Added get_mode
-Added PI_TIME_RELATIVE
-Added PI_TIME_ABSOLUTE
-Added get_servo_pulsewidth
-Added set_servo_pulsewidth
-Added time_sleep
-Added pigpio_start
