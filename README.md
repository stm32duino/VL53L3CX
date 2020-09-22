# VL53L3CX
The VL53L3CX is the latest Time-of-Flight (ToF) product from STMicroelectronics and embeds ST’s third generation FlightSense patented technology. It combines a high performance proximity and ranging sensor, with multi target distance measurements and automatic smudge correction. The miniature reflowable package integrates a single photon avalanche diode (SPAD) array and physical infrared filters to achieve the best ranging performance in various ambient lighting conditions, with a wide range of cover glass windows.

# API
This sensor uses I2C to communicate. And I2C instance is required to access to the sensor.

The API provides simple distance measure, single swipe gesture detection, directional (left/right) swipe gesture detection and single tap gesture detection.

# Examples

There are 2 examples with the VL53L3CX library.

To use these examples you need to connect the vl53l3cx sensor directly to the board.
instructions to connect the pins of vl53l3cx to the board:
- pin 1 (Interrupt) connected to pin A2 
- pin 2 (SCL_I) connected to pin SCL with a 4kiloohm resistor
- pin 3 (XSDN_I) connected to pin A1
- pin 4 (SDA_I) connected to pin SDA with a 4kiloohm resistor
- pin 5 (VDD) connected to 3.3V VDD
- pin 6 (GND) connected to GND
- pins 7,8,10,9 are not connected.

* VL53L3CX_Sat_HelloWorld: This example code is to show how to get multi-object detection and proximity values of the VL53L3CX satellite sensor in polling mode.

* VL53L3CX_Sat_HelloWorld_Interrupt: This example code is to show how to get multi-object detection and proximity values of the VL53L3CX satellite sensor in interrupt mode.

# Note
The VL53L3CX is a fully integrated miniature module with a low power microcontroller with advanced digital firmware. Detection with full field of view (FoV) is up to 300 cm +. It works with many types of glass roofing materials. Xshutdown (reset) and stop GPIO are integrated to optimize remote operation.

# Documentation
You can find the source files at

https://github.com/stm32duino/VL53L3CX

The VL53L3CX datasheet is available at

https://www.st.com/content/st_com/en/products/imaging-and-photonics-solutions/proximity-sensors/vl53l3cx.html
