# nRF52-DK and LSM9DS1

This is redefined main.c from SDK folder: $SDK/examples/peripheral/twi_sensor/


* Should be added include file from: https://github.com/STMicroelectronics/STMems_Standard_C_drivers/tree/master/lsm9ds1_STdC/driver


* example code from STM is: https://github.com/STMicroelectronics/STMems_Standard_C_drivers/tree/master/lsm9ds1_STdC/example

## Note for Segger studio: 

printf should be enabled in: right mouse *click on project* > *Options* > choose *Common* > in search box type "float" > change *Printf Floating Point Supported* from "No" to "Float".

## Hardware required
* nRF52 DK (PCA10056)
* LSM9DS1 module steval-mki159v1 like: https://www.st.com/en/evaluation-tools/steval-mki159v1.html

## Connect modul and nRF52
JP1 on STEVAL     nRF52 DK
-------------   ------------
1, 2            VCC  
21 (SDA)        0,26  
20 (SCL)        0,27  

