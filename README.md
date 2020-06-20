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

As of June 2020, the latest Operating System is Raspberry Pi OS, with Raspberry Pi 4B, 
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
- Added many error constants (over 150)
- Added gpio_read method
- Added gpioSetPullUpDown method and constants

v1.3 (29 May 2020)
- Added gpioInitialise
- Added hardware_PWM
- Added gpioPWM
- Added gpioSetPWMRange

v1.4 (31 May 2020)
- Added gpioSetPWMFrequency
- Added gpioTerminate
- Added get_mode
- Added PI_TIME_RELATIVE
- Added PI_TIME_ABSOLUTE
- Added get_servo_pulsewidth
- Added set_servo_pulsewidth
- Added time_sleep
- Added pigpio_start

v1.5 (3 June 2020)
- Added PI_LOW
- Added PI_HIGH
- Added #Pragma to gpioSetPullUpDown

v1.6 (7 June 2020)
 - Added 13 pigif_ error constants
 - Added other constants
 - Added gpioTick
 - Added callback
 - Added callback_ex
 - Added pigpio_error
 - Added time_time
 - Added pigpiod_if_version
 - Added pigpio_stop
 
 v1.7 (8 June 2020)
 - Added set_PWM_dutycycle
 - Added gpioGetPWMdutycycle
 - Added get_PWM_dutycycle
 - Added set_PWM_range
 - Added get_PWM_range
 - Added get_PWM_real_range
 - Added set_PWM_frequency
 - Added get_PWM_frequency
 - Added notify_open
 - Added notify_begin
 - Added notify_pause
 - Added notify_close
 - Added set_watchdog
 - Added set_glitch_filter
 - Added set_noise_filter
 - Added read_bank_1
 - Added read_bank_2
 - Added clear_bank_1
 - Added clear_bank_2
 - Added set_bank_1
 - Added set_bank_2
 - Added hardware_clock
 - Added hardware_PWM
 - Added get_current_tick
 - Added get_hardware_revision
 - Added get_pigpio_version
 - Added wave_clear
 - Added wave_add_new
 - Added wave_add_generic
 - Added wave_add_serial
 - Added wave_create
 - Added wave_delete
 - Added wave_send_once
 - Added wave_send_repeat
 - Added wave_send_using_mode
 - Added callback_cancel
 - Added wait_for_edge
 - Added bsc_xfer 
 - Added bsc_i2c
 - Added event_callback
 
V1.8 (11 June 2020)
 - Added event_callback_ex
 - Added event_callback_cancel
 - Added wait_for_event

V1.9 (12 June 2020)
 - Updated hardware_PWM

v1.10 (13 June 2020)
 - Modified gpioInitialize to handle errors

V1.11 (14 June 2020)
 - Added more constants (RISING_EDGE, FALLING_EDGE, EITHER_EDGE)
 - Modified gpioSetISRFunc function 
 - Added i2c_open
 - Added i2c_close
 - Added i2c_write_byte
 - Added i2c_write_byte_data
 - Added i2c_read_word_data
 - Updated Constructor and add the correct call order in Open event
 
V1.12 (16 June 2020)
 - Added i2c_Read_Byte_Data

V1.13 (19 June 2020)
 - Added gpioTime
 - Added gpioSetAlertFunc
 - Added gpioSetWatchdog
