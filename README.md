The Touchlib library contains 2 classes that work differently, one reads the voltage level on an analog pin, the other counts till the pin goes high.


Features:
- Features a very responsive DigitalTouch calass (Should work on any digital I/O)
- Also features a less responsive but higher resolution and more compact AnalogTouch class (only works on 10 bit analog input that can also be set up as digital I/O)
- Both Classes are minimalistic, and have the same methods to make it easy to use, but they different defaults, and work differently under the hood.
- They both provide boolean, and byte readings, both have calibrate, and hysteresis methods, to make sure all the readings are accurate and stable.

Note that: The value given by DigitalTouch::Read() method rises when touched, while the value given by the AnalogTouch::Read() method falls when touched!

Hardware requirements:
- Arduino running at 16MHz (Any type should do. 16MHz is important because of timing. 8MHz will work but require different settings. Mine is pro-mini 5V, 16MHz version.)
- 2 Touch pads hooked up to any digital I/O or any 10 bit analog input that can also be set up as digital I/O in both case with an external 1M pullup resistor to VCC.
  (Unlike the CapacitiveSensor library this one does not require an extra pin to operate! 1 pin as touch input with an external 1M pullup resistor. That's it!)


Software requirements:
- Arduino IDE
- TouchLib library (This one...)


Skill requirements:
- You need to have basic arduino skills. (Soldering, understanding arduino code, installing and using libraries, etc. This is a library of source code and CAD files with an example sketch not a tutorial, so I won't explain everything here.)


Instructions:
1. Add library to your arduino IDE 
 - Open terminal in your Arduino/libraries directory, and run "git clone https://github.com/RPBCACUEAIIBH/TouchLib" and restart the IDE.
 - Download as .zip package, go to the Sketch/Include Library/Add .ZIP Library... in you Arduino IDE, select it, and click ok.
2. Open the included example sketch to see how to use it.

[If you find this useful, please consider donationg.](http://osrc.rip/Support.html)
