# IOT PROJECT: TEMPERATURE DATA ON FIREBASE 


## AIM

To create a Firebase project with a realtime database and to store the temperature and humidity reading of DHT11 in the database using the ESP8266 interfaced with LCD 16x2 I2C.


## COMPONENTS

1.	ESP8266 NodeMCU
2.	LCD 16x2 I2C
3.	DHT11
4.	Jumper Wire
5.	USB cable


## CONNECTION

### LCD16x2 I2C Module Pin Diagram

 ![ii2c module](https://github.com/user-attachments/assets/5d0150be-5a9b-4462-ba5f-d3870d4c020a)

<br> VCC = power supply ---->  3V3
<br> GND = ground          ---->  GND
<br> SDA = serial data line   ---->  D2
<br> SCL = serial clock line   ---->  D1

### DHT11 Pin Diagram

 ![DHT11](https://github.com/user-attachments/assets/73f3e446-f3df-43a1-8db5-17e8f8b26365)

<br> S     = Output     ---->  D4
<br> VCC   = power supply  ---->  3V3
<br> GND   = ground   ---->  GND


## PROCEDURE

<br> Step 1 : Interface ESP8266 microcontroller to Visual Studio Code using port.
<br> Step 2: Interface ESP8266 microcontroller with DHT11 and print temperture and humidity values on serial monitor.
<br> Step 3 : Interface ESP8266 microcontroller with LCD 16x2 I2C to display HI on LCD
<br> Step 4 : Interface ESP8266 microcontroller with LCD 16x2 I2C and DHT11 by modifying both the programs.
<br> Step 5 : Install the Firebase-ESP-Client Library.Then, program the ESP8266 to Interface with Firebase
<br> Step 6 : Need to insert your network credentials, URL database, and project API key for the project to work.


## PROBLEMS FACED

### Error 1 -   library installation

<br> How to rectify:
<br> (1)  Need to find suitable library
<br> (2)  Copy  link address of libraries mentioned below -> paste next to "lib_deps =" on platformio.ini file in visual studio code

### Error 2 -   Not getting DHT22 sensor reading 

<br> How to rectify:
<br> (1)  On serial monitor it prints like
<br> &ensp;&ensp;&ensp;&ensp;  Humidity: nan %  Temperature : nan*C      // not getting the readings 
<br> (2)  Changed sensor , this error shows because of sensor complaint.


## OUTPUT

![IMG_1](https://github.com/user-attachments/assets/21adf079-b9be-431c-b5d6-8a917927456c)


## REFERENCES

For Visual Studio Code, the libraries are,
<br> lib_deps = 
&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;bonezegei/Bonezegei_DHT11@^1.0.1
&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;marcoschwartz/LiquidCrystal_I2C@^1.1.4
&ensp;&ensp;&ensp;&ensp;&ensp;&ensp;mobizt/Firebase Arduino Client Library for ESP8266 and ESP32@^4.4.14 



