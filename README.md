# nRF52-DK and LSM9DS1

This is redefined main.c from SDK folder: $SDK/examples/peripheral/twi_sensor/


* Should be added include file from: https://github.com/STMicroelectronics/STMems_Standard_C_drivers/tree/master/lsm9ds1_STdC/driver


* example code from STM is: https://github.com/STMicroelectronics/STMems_Standard_C_drivers/tree/master/lsm9ds1_STdC/example

### Note for Segger studio: 

printf should be enabled in: right mouse *click on project* > *Options* > choose *Common* > in search box type "float" > change *Printf Floating Point Supported* from "No" to "Float".

### Hardware required
* nRF52 DK (PCA10056)
* LSM9DS1 module steval-mki159v1 like: https://www.st.com/en/evaluation-tools/steval-mki159v1.html

### Connect modul and nRF52
|JP1 on STEVAL   |  nRF52 DK|
|-------------   |------------|
|1, 2|            VDD  |
|21 (SDA) |       P0.26  |
|20 (SCL) |       P0.27  |
|GND|       GND  |

### Output example 
```
TWI device example started.
Who am I register [IMU]: 0x68 [MAG]: 0x3d 
IMU - [mg]:7.44	-953.06	-361.49	[mdps]:560.00	-1330.00	-1190.00
MAG - [mG]:590.44	1506.26	-253.46
IMU - [mg]:7.20	-953.67	-365.76	[mdps]:-700.00	1610.00	1470.00
IMU - [mg]:6.95	-953.06	-368.56	[mdps]:-4830.00	10920.00	9310.00
IMU - [mg]:6.95	-952.33	-368.93	[mdps]:3010.00	-7420.00	-6790.00
IMU - [mg]:7.08	-952.70	-371.25	[mdps]:24290.00	-56210.00	-48020.00
IMU - [mg]:7.81	-952.09	-372.34	[mdps]:27860.00	-61740.00	-51380.00
IMU - [mg]:6.95	-953.19	-371.37	[mdps]:7420.00	-11480.00	-7840.00
MAG - [mG]:581.16	1519.02	-249.98
IMU - [mg]:7.20	-953.92	-372.34	[mdps]:-4480.00	16870.00	15960.00
....
```

