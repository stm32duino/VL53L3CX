# VL53L3CX
Arduino library to support the VL53L3CX Time-of-Flight ranging sensor with advanced multi-object detection.

## API

This sensor uses I2C to communicate. And I2C instance is required to access to the sensor.
The APIs provide simple distance measure and multi-object detection in both polling and interrupt modes.

## Examples

There are 2 examples with the VL53L3CX library.

In order to use these examples you need to connect the VL53L3CX satellite sensor directly to the Nucleo board with wires as explained below:
- pin 1 (Interrupt) of the VL53L3CX satellite connected to pin A2 of the Nucleo board 
- pin 2 (SCL_I) of the VL53L3CX satellite connected to pin D15 (SCL) of the Nucleo board with a Pull-Up resistor of 4.7 KOhm
- pin 3 (XSDN_I) of the VL53L3CX satellite connected to pin A1 of the Nucleo board
- pin 4 (SDA_I) of the VL53L3CX satellite connected to pin D14 (SDA) of the Nucleo board with a Pull-Up resistor of 4.7 KOhm
- pin 5 (VDD) of the VL53L3CX satellite connected to 3V3 pin of the Nucleo board
- pin 6 (GND) of the VL53L3CX satellite connected to GND of the Nucleo board
- pins 7, 8, 9 and 10 are not connected.

* VL53L3CX_Sat_HelloWorld: This example code is to show how to get multi-object detection and proximity
  values of the VL53L3CX satellite sensor in polling mode.

* VL53L3CX_Sat_HelloWorld_Interrupt: This example code is to show how to get multi-object detection and proximity
  values of the VL53L3CX satellite sensor in interrupt mode.

## Note

The VL53L3CX is a fully integrated miniature module with a low power microcontroller with advanced digital firmware.
Detection with full field of view (FoV) is up to 300 cm +. It works with many types of glass roofing materials.
Xshutdown (reset) and stop GPIO are integrated to optimize remote operation.

## Documentation

You can find the source files at
https://github.com/stm32duino/VL53L3CX

The VL53L3CX datasheet is available at
https://www.st.com/content/st_com/en/products/imaging-and-photonics-solutions/proximity-sensors/vl53l3cx.html
