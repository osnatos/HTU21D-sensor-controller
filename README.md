# HTU21D-sensor-controller
The sensor controller is designed to work with the [HTU21D sensor](https://www.te.com/commerce/DocumentDelivery/DDEController?Action=showdoc&DocId=Data+Sheet%7FHPC199_6%7FA6%7Fpdf%7FEnglish%7FENG_DS_HPC199_6_A6.pdf%7FCAT-HSC0004),using the Sensor Controller Engine of CC2640R2F MCU. 
* Project name: HTU21D sensor 
* Project file: HTU21D_sensor.scp 
* Operating system: TI-RTOS 
* Target chip: CC2640R2F, package QFN48 7x7 RGZ 
* I2C0_SCL - pin 11; I2C0_SDA - pin 10
# How to generate project files.
In order to generate all project files, you must:
* Launch “Sensor Controller Studio” (SCS) using the  HTU21D_sensor.scp project file.
* In the SCS program, click on the “Code Generator” button. SCS will create a scif_files folder (if it did not exist before) and generate all the necessary files in it (except for the readme file).
* The file “scif_htu21d_how_to_use.html” contains information on using the controller.
# Software tools:
* Sensor Controller Studio v2.7.0.155
# Debugging:
* The project was debugged on the CC2640R2-LAUNCHXL debug board.
# Connection to CC2640R2-LAUNCHXL board:
* HTU21D / pin1 - SDA / DIO5 + PULUP 10K
* HTU21D / pin2 - GND
* HTU21D / pin5 - 3.3V
* HTU21D / pin6 - SCL / DIO4 + PULUP 10K
# Used in the project:
* The controller was used in the [Beacon_CC2640_with_SensorController_HTU21D](https://github.com/osnatos/Beacon_CC2640_with_SensorController_HTU21D).

