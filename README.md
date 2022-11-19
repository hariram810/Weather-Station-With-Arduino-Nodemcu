# Weather-Station-With-Arduino-Nodemcu

![1](https://user-images.githubusercontent.com/118633170/202869345-86c7b9bf-c057-46bc-9f13-ff3e48c0f1d3.jpg)


This is a simple weather station made under 20$ to get data from the devices and display to the internet and make calculations regarding that

If you have hard-time 3d printing stuff and other materials which i have provided in this project please refer the professionals for the help, JLCPCB is one of the best company from shenzhen china they provide, PCB manufacturing, PCBA and 3D printing services to people in need, they provide good quality products in all sectors


Please use the following link to register an account in JLCPCB

https://jlcpcb.com/RNA

![1](https://user-images.githubusercontent.com/118633170/202869382-921514c1-dbbf-4a28-bbdd-0c1f9025de24.jpg)

![2](https://user-images.githubusercontent.com/118633170/202869365-6cf6277b-8590-4943-9c2f-4b4b74a5d1ba.jpg)


Pcb Manufacturing

----------

2 layers

4 layers

6 layers



PCBA Services

JLCPCB have 350k+ Components In-stock. You don’t have to worry about parts sourcing, this helps you to save time and hassle, also keeps your costs down.

Moreover, you can pre-order parts and hold the inventory at JLCPCB, giving you peace-of-mind that you won't run into any last minute part shortages.



3d printing

-------------------

SLA -- MJF --SLM -- FDM -- & SLS. easy order and fast shipping makes JLCPCB better companion among other manufactures try out JLCPCB 3D Printing servies

JLCPCB 3D Printing starts at $1 &Get $54 Coupons for new users


This Weather Station Uses Arduino ,Python & Nodemcu Along With Different Analog Value Sensor & Digital Value Sensors. Since Nodemcu Have Only One A0 Pin & We Need Values From Different Analog Sensors Like :-


SMOKE

Gas Sensor(MQ2) module is useful for gas leakage detection (home and industry). It is suitable for detecting H2, LPG, CH4, CO, Alcohol, Smoke or Propane. Due to its high sensitivity and fast response time, measurement can be taken as soon as possible. The sensitivity of the sensor can be adjusted by potentiometer.


CNG

This is a very easy to use low cost semiconductor Gas sensor Module with analog and digital output. This module uses MQ3 Alcohol gas sensor as a alcohol gas sensing element. It requires no external components just plug in Vcc & ground pins and you are ready to go.


RAIN

The rain sensor works on the principle of total internal reflection. ... An infrared light beams at a 45-degree angle on a clear area of the windshield is reflected and it is sensed by thesensor-inside the car. When it rains, the wet glass causes the light to scatter and lesser amount of light gets reflected back to the sensor

An additional application in professional satellite communications antennas is to trigger a rain blower on the aperture of the antenna feed, to remove water droplets from the cover that keeps pressurized and dry air inside the wave-guides.


TEMPERATURE & HUMIDITY

This is a calibrated digital temperature and humidity module with onboard sensor DHT22 (AM2302), which features higher accuracy and a wider measuring range than DHT11.It can be used for detecting ambient temperature and humidity, through the standard single-wire interface.


LIGHT

LDR (Light Dependent Resistor) as the name states is a special type of resistor that works on the photoconductivity principle means that resistance changes according to the intensity of light


PRESSURE & ALTITUDE

The BMP280 is an absolute barometric pressure sensor, which is especially feasible for mobile applications. Its small dimensions and its low power consumption allow for the implementation in battery-powered devices such as mobile phones

                  Step 1: Parts Needed
                  
The Parts Needed for the project are the following



Arduino Nano

ESP8266

MQ-2

MQ-5

MQ-6

MQ-7

DHT22

Rain Sensor

Light Sensor

![3](https://user-images.githubusercontent.com/118633170/202869428-8a4704e8-dfb4-4a57-b4d5-552c421d86c0.jpg)
![4](https://user-images.githubusercontent.com/118633170/202869454-92677f63-5e68-4c8b-8978-3811e09e73b4.jpg)
![5](https://user-images.githubusercontent.com/118633170/202869460-a55e4d23-0734-4380-a01e-afd76d28cc51.jpg)
![6](https://user-images.githubusercontent.com/118633170/202869461-aa326600-fc3b-4866-8008-3fe3e97fcbf5.jpg)
![7](https://user-images.githubusercontent.com/118633170/202869466-d72cee0c-2d93-44a6-a4b1-e274e1ba08ea.jpg)


 Use ArduinoJson Library To Sent Values Collected From Sensors Via Arduino As "DOC" & Print It In Nodemcu Serial Monitor , Thats One-Way To Show Multiple Analog Readings In Nodemcu Board .
 
           Step 2:

I Use This Arduinojson 6.13.0 Library For SERIAL MONITOR DATA -- BLYNK -- THINGSPEAK -- IFTTT & UBIDOTS

Then I Use This Arduinojson 5.13.1 Library For FIREBASE , ADAFRUIT-IO Other Arduinojson Library Does Not Work Beacuse I Use DynamicJsonDocument doc(1024); For Converting Data From Arduino To Nodemcu It Is An Arduinojson 6.13.0 Variant & Not Yet Compactable With FirebaseArduino.h & Adafruit_MQTT.h Library , So I Have Downgraded To This Arduinojson 5.13.1 Library . I Need To Do Some Tweeks In The Code To Make It All Work & All The Arduino Files Have Been Updated In The Repository

          Step 3:
When we work on Arduino we typically use Arduino IDE (Integrated development environment), which is software that's available for all major computers which provide a text editor for writing code with integrated library support and a physical programmable circuit board to run the code.

The Arduino programming language is a modified version of C/C++. Usually, we program in C++ with the addition of methods and functions. A program written in Arduino programming language is called sketch and saved with .ino extension. You can even use Python to write an Arduino program. All these languages are text-based programming languages.

          Step 4:
1. Download & install the Arduino environment (IDE)
If you just got your Arduino Uno board, you’ll first have to install the Arduino IDE (Integrated Development Environment) on another computer. The code is typed into the IDE and sent to the Arduino via a USB cable.

Visit arduino.cc to download the most recent Arduino IDE version for your computer. There are different versions for Mac, Windows, and Linux OS.

At the download page, click on the “Installer” option for the easiest installation then

Save the .exe file to your disk drive.
Open the .exe file.
Click the button to agree to the licensing agreement
Decide which components to put in, then click “Next”
Select which folder to put in the program to, then click “Install”
Wait for the program to complete installing, then click “Close”
2. Launch the Arduino IDE

After your Arduino IDE software is downloaded, unzip the folder. To do so, double-click on the Arduino shortcut on your Desktopt. The IDE will open up and you’ll see the code editor.

![345](https://user-images.githubusercontent.com/118633170/202869513-05afacc0-591b-4906-950f-06c61816ca6c.jpg)
![44](https://user-images.githubusercontent.com/118633170/202869515-8a7d670d-fef5-48c9-911a-29427c334cbb.jpg)
![df](https://user-images.githubusercontent.com/118633170/202869517-86ad91c5-b057-4269-8b17-cce45151a9c7.jpg)




3. If needed, install the drivers
If you used the Installer, it'll install drivers automatically as soon as you connect your board.



4. Connect the board to your computer via the USB cable
To power up your board, connect your Arduino board with the pc via USB cable. The green color power LED should glow on the board.



   5. Select your board
Next, make sure the software is ready up for your particular Arduino board. Go to the “Tools” computer menu from the menu bar. Select the “Board” option and another menu will appear, where you'll select your Arduino model from the list.

    6. Select your serial port
Select the serial device of the Arduino board. Go to Tools, and then the serial port menu. You might see COM3 or higher (COM1 and COM2 are usually reserved for hardware serial ports). To find out which port your Arduino board is connected to, disconnect your Arduino board and re-open the menu. The entry that disappears should be the Arduino board. Reconnect the board and choose that serial port.


Step 5: Trouble Shooting

Trouble Shooting

ESP8266-BOARD VERSION ERROR
Change The ESP8266-BOARD VERSION From Latest To esp8266-2.7.4
SSL-FINGER-PRINT ERROR

This issue is attributed to Arduino IDE Boards Manager not cleaning up previous package installation before a new one is applied. As this is not done, then it is user responsibility to remove previous package before applying a new one.

To prevent it from happening, if you are changing between staging and stable, first press Remove button to delete currently used installation.


There is no need to remove the installed package if you are changing it to another version (without switching between staging and stable).



Navigate further down to Arduino15\packages\esp8266\hardware\esp8266 directory. Inside you will find two folders with different esp8266 / Arduino package installations.


Delete the older folder. Restart Arduino IDE, select your ESP module and the error should be gone.
Note: If you are not sure which folder to delete, then remove both of them. Restart Arduino IDE, go to Tools > Board: > Boards Manager and install the esp8266 / Arduino package again. Select ESP8266 module and the issue should be resolved.

Download the pcb files from here :-- https://bit.ly/3hVeRxw
