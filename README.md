
# [Maker Drive](https://www.cytron.io/p-maker-drive-simplifying?tracking=b-py-h-bridge-motor-driver-for-beginner) MicroPython Library for [Pi Pico](https://www.cytron.io/p-maker-pi-pico?tracking=b-py)
This library supports Maker Drive to be used with Pi Pico

**The library file must be saved inside the Raspberry Pi Pico before uploading user's code**
## Add Library
Step 1: Download the library file (motor_driver.py)

Step 2: Launch Thonny application and open the library file

![11](https://user-images.githubusercontent.com/34527010/106845087-2210c380-66e5-11eb-9d72-5d9219a878f1.PNG)


Step 3: Save the library file into the Pi Pico

![12](https://user-images.githubusercontent.com/34527010/106845132-381e8400-66e5-11eb-9cc1-a20fabf47f16.png)

![13](https://user-images.githubusercontent.com/34527010/106845126-36ed5700-66e5-11eb-88a6-5623e85f4e8d.png)


Step 4: Save the library with the same name you downloaded with (motor_driver.py) **Must add .py at the back**

![14](https://user-images.githubusercontent.com/34527010/106845128-381e8400-66e5-11eb-80bd-24fbd42bff8b.PNG)


Click OK and the library is added to your Pi Pico

## Import motor_driver library

 - Import motor_driver library
 `from  motor_driver  import  *`

## Create object for motor_driver

 -   Create object using the class
 - motor_driver(M1A,M1B,M2A,M2B)
 `motor  =  motor_driver(4,5,2,3)`
	 - M1A = 4, M1B = 5, M2A = 2, M2B = 3

## Set motor speed and direction

 - Positive value indicates forward direction with 100 as full speed
 - Negative value indicates backward direction with -100 as full speed
 - 0 stops the moto
 
**Move Forward**

 - `motor.speed(50,50) # move forward at speed 50`
 
**Move Backward**

 - `motor.speed(-50,-50) # move backward at speed 50`

**Turn Left**

 - `motor.speed(0,50) # turn left at speed 50`

**Turn Right**

 - `motor.speed(50,0) # turn right at speed 50`

**Brake**

 - `motor.brake() # brake the motor`

