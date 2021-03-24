# Security-System
Door Locker Security System consists of two ECU’s. The first ECU called HMI responsible for interfacing with the user and the second ECU called control ECU which is responsible for the system operations and control. In the project I implemented the following drivers Keypad, LCD, DC Motor, UART, Timer, I2C and External EEPROM.

description:
in simulation project, there is keypad to take password and lcd to display the orders and info to the user.. in the beginning we write the password twice to make matching and save it in EEPROM then we move to step 2 which displays two options the first is, *: open door and this requires writing password twice to make sure that's right.
if match >> motor rotates clockwise for 15 sec then stops for 3 sec then rotates back anti-clock wise for 15 sec.
if its not matching >> user will try for 3 times after that system will stop for 1 minute while buzzer will work.
The second option is, #: Change Password.
in this we write old password and new password twice then its changed 
if user entered old pass wrong for  3 times, system will stop and buzzer will work for 1 minute.
if user entered new pass wrong it will keep him entering it till its matched.
