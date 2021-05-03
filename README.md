## USB to UART converter with isolation barrier

The project was created for safe debugging of power converters and other devices operating with high voltage through the UART interface using the _printf_ function. For isolation, a digital isolator from Texas Instruments - _ISO7721DR_ with isolation voltage up to 1500V was chosen. The main converter is the popular _CP2102_ chip from Silabs.

The converter can use with microcontrollers and other devices with a logic level of 3.3V (STM32 and others) and 5V (ATmega and others), which makes it universal. Leveling is done by supplying voltage from the main board to the converter (VREF pin).

![3D view](https://habrastorage.org/webt/4p/82/lq/4p82lqaxkefubuul_a-x5edehsq.png)

## Features:

* Type converter: *USB -> UART*
* Used IC: *CP2102*
* Isolation voltage: *1000 V*
* Logic level: *2.5, 3.3 and 5V*
* Temperature ranges: *-40...+85°С*

## Project structure:

* Hardware
    * docs - documentation for project: ВОМ, schematic, etc
    * hardware - source project for design PCB
    * manufacture - gerber files for order PCB
    * mechanical - source project for 3D design

## Assembly drawing

![Assembly drawing](https://habrastorage.org/webt/sc/ni/yn/scniynm_reas2cklmnus6nzhmgg.png)

## Bill of materials

![BOM](https://habrastorage.org/webt/lp/ez/pp/lpezppswlglgllcdok7hqcqlnf0.png)

## License

All source files for the project are distributed under the [MIT](./LICENSE "Text of license") license and you can use the project for commercial activities. But you need remembering that the author of the project does not give any guarantees for the operability of the device or parts of the project and also does not bear no liability for claims or damages.