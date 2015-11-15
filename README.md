# rcjoystick

The aim of the project is use a standard RC Controller and a Orange RX receiver to control RC Model games.

I followed the following blog http://sjtrny.com/posts/2015/1/26/interfacing-an-rc-radio-with-your-computer.html

Tested with the following hardware :
- Arduino Uno SMD
- DX6i Spektrum rc transmitter

For the following games :
- FPV Freerider
- Liftoff

# Install on Mac

```
$ sudo port install dfu-programmer
```

Add 2 libraries to Arduino toolkit :
- UnoJoy - https://github.com/AlanChatham/UnoJoy
- PinChangeInt - https://code.google.com/p/arduino-pinchangeint/downloads/detail?name=pinchangeint-v1.72.zip

Touch the connector 5 and 6 on the Arduino

```
$ git clone https://github.com/AlanChatham/UnoJoy.git
$ cd UnoJoy/UnoJoy
$ vim TurnIntoAJoystick.command  # Update path for dfu-programmmer
$ bash TurnIntoAJoystick.command

Abracadabra!

Trying to program for Arduino Uno R1/R2...
Validating...
2778 bytes used (67.82%)

Unplug your Arduino and plug it back in. It's a joystick now!
```