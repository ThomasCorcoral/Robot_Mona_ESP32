# Mona Robot Library for P-ANDROIDE (2021-2022, spring semestre)

## Description
Library to use the MONA ESP32 robot with the Arduino IDE
## Installation
### Arduino IDE
Install the last Arduino IDE version (curretly working on 1.8.19). The current version is at the [Arduino website](http://www.arduino.cc/en/main/software).

### ESP32 compatibility with the Arduino IDE
Follow the instructions on the :
- Start Arduino IDE and open File > Preferences window.
- Into the  *Additional Board Manager URLs* field, enter the following release link. You can add multiple URLs, separating them with commas. 
  + `https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json`
- Click 'Ok' to close the Board Preferences Window. Open Boards Manager from Tools > Board > Board Manager. Search for *esp32*, select the option from  Espressif Systems and install it. 
- After the instalation has finished, go to Tools > Board and select *ESP32 Wrover Module*

### Adding the MONA-ESP library to Arduino IDE
To install the MONA-ESP library into the Arduono IDE follow the next steps:
- Scroll up in this webpage, click the green button on the top right of the page with the text *Clone or Download*. Choose Download as Zip. 
- From the Arduino IDE, go to Sketch > Include Library > Add .ZIP Library . Browse and find the downloaded Zip file, select and install.

### Installing External Libraries
The MONA-ESP code depend on external libraries to control some of the peripherals of the board. To compile and use the MONA-ESP libraries it is necessary to install some dependencies. For that, within the Arduino IDE go to Tools > Manage Libraries
Search for and install the following libraries:
- Adafruit LSM9DS1
- Adafruit MCP23008
- Adafruit Neopixel
- Adafruit Unified Sensor

### Testing the Library
Once the libraries have been installed, from the Arduino IDE select File > Examples > MONA-ESP Robot Library and select one of the examples. Ensure that the board *ESP32 Wrover Module* has been selected (From Tools > Board). Connect the MONA-ESP robot to the compter through the USB cable and click Upload. 
