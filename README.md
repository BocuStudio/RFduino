# RFduino: An Arduino shrunk to the size of a finger-tip and made wireless!

![logo](https://raw.github.com/RFduino/RFduino/master/4up%20image.jpg)

[Video](http://www.youtube.com/watch?v=arWBdGwCJcM)  

## Installation

* Get the [RFduino hardware](http://RFduino.com).

* Install the [FTDI drivers](http://www.ftdichip.com/Drivers/VCP.htm).

* Download [Arduino 1.6.3](http://arduino.cc/en/Main/Software) or newer.
  * _Mac OS X_: Requires Java 6 to be installed. Available [here](https://support.apple.com/kb/DL1572?locale=en_US).

* Open Arduino
  * Either, edit preferences, and add rfduino.com as the Server (HTTP) under Proxy Settings and save.
      ![preferences](preferences.png)
  * OR, if you are using Arduino 1.6.4 or newer, then there is now another way to do this. With preferences open, instead of putting rfduino.com as the Server proxy, you can add the JSON file to "Additional Boards Manager URLs:". From this depo, that URL is: https://raw.githubusercontent.com/BocuStudio/RFduino/master/package_rfduino_index.json
  * Open the Boards Manager under Tools->Board menu.
  * Select the RFduino package at the end of the list, and click Install to install it.
  * Your new board will now show up in the Tools->Board menu.

Select the board and port, and you're ready to go!

## Linux

```
// FTDI drivers are not needed (they are built into the kernel)
wget http://downloads.arduino.cc/arduino-1.6.3-linux64.tar.xz
tar -xf arduino-1.6.3-linux64.tar.xz

Ubuntu: sudo apt-get install default-jre
Fedora: sudo yum install jre
OpenSUSE: sudo zypper install jre

// otherwise the com port open will fail with permission denied (you must logout/login for change to take effect)
sudo usermod -aG dialout <username>
```

## Getting Started

* Attach the USB shield

* Select RFduino from the ```Tools/Board``` menu

* Select the port from the ```Tools/Port``` menu

* Select an example from the ```Files/Examples/RFduinoNonBLE``` or ```Files/Examples/RFduinoBLE``` directory

* Select ```Upload``` to compile, upload and execute the sketch

* Download the iPhone example apps from the iPhone App Store (search for ```RFduino```).
    * Detailed instructions for the Temperature app are available [here](http://files.rfdigital.com/rfduino.temperature.guide.pdf).
    * Detailed instructions for the ColorWheel app are available [here](http://files.rfdigital.com/rfduino.rgb.colorwheel.guide.pdf).

## RFduinoApps

Check out the [RFduinoApps](http://github.com/RFduino/RFduinoApps) repository for iPhone App source code & RFduino to Raspberry Pi integration projects.

# Communicating with us

The best way to communiate with us is on the [RFduino Forum](http://forum.RFduino.com).
