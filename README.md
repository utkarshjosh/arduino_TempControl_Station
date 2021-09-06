## Temperature Regulating Device
## BIRBY

Birby is a arduino-nano powered temperature regulator for a local environment intended for pet birds at home.
The device monitors atmosphere and updates the details on a OLED screen
Displaying humidity and temperature and the state of a cooling Fan and a Heating Lamp



### Sensor
The device is powered by ultra low-cost DHT-11 temperature and humidity sensor that connects at digital pin 2 and uses standard DHT library

### Oled Display
The Oled Display used is 0.96inch I2C , the device welcomes with a loading screen animation, displaying the title of the project.
That bitmaps for it has been designed with the help of a youtube channel -[Volos Project](https://www.youtube.com/watch?v=0KGMFhFQ0YY) <br>
**Caution:** Bitmap arrays takes memory, so which limits the ability to put more logic in code and we have to make reduction in use of lot of bitmaps arrays to make enough space for rest of code.

### User Input
There are two input buttons, mode and set
MODE button: Is used to toggle to settings menu and then higher temperature range and then lower temperature range and then back to home screen.
SET button: Is used to increment the temeprature offset values , until it trips back to its lowest value. 
Changing the values with SET buton and then pressing the MODE button to come back to home screen saves the offsets to EEPROM.
EEPROM update function is used to do least amounts of writes on the memory.


### Relays 
The device uses 1 Channel 5V Relay Module and regualtes Relays when the temparature crosses the set limits.

### Breadboard Setup
![image](https://github.com/utkarshjosh/arduino_TempControl_Station/blob/master/breadboard-setup.jpeg?raw=true)
<br><br>
![image](https://github.com/utkarshjosh/arduino_TempControl_Station/blob/master/Home-Sceen-diplay-on-breadboard.jpg?raw=true)

<br><br>
[![Watch the video]](https://raw.githubusercontent.com/utkarshjosh/arduino_TempControl_Station/master/Booting-animations.mp4)


### Final Device Protype
![image](https://github.com/utkarshjosh/arduino_TempControl_Station/blob/master/final-device-prototype.jpg?raw=true)
<br> <br>


![image](https://github.com/utkarshjosh/arduino_TempControl_Station/blob/master/diagram.png?raw=true)

