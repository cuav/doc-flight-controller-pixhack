### Introduction{#介绍 }

---
Pixhawk is the world's most famous open source flight control hardware manufacturer 3DR launched open source flight control. Pixhawk as an open source hardware and has powerful features, reliable performance has been favored by the majority of users. The open source of hardware has caused many hardware manufacturers to join the ranks of manufacturing pixhawk. As the well-known open source flight control manufacturer in China, cuav uses the same hardware design and fully imported chips according to the original pixhawk design to produce the cuav. Pixhawk has a very high stability.

#### Cover all models{#覆盖全机型}
The Pixhawk is a drone control system that runs [PX4](http://px4-travis.s3.amazonaws.com/Firmware/master/px4fmu-v5_default.px4) and [ArduPilot](http://firmware.ardupilot.org) environments.

Applicable model: plane\copter\helicopters\VTOL\unmanned vehicles\ unmanned boats.

#### Powerful processor {#强大处理器}

Based on STM32F427 (180MHZ) master and STM32F100 coprocessor.

####Redundant design {#冗余设计 }

* Built-in two-group IMU redundancy design (including two groups of accelerometers, two groups of gyroscopes, one group of electronic compasses, and one group of digital barometers)

* Support 3 sets of power supply redundant switch

* Software built-in sensor data fusion mechanism and failover mechanism will greatly reduce the chance of crash caused by flight control.
#### Rich expansion {#丰富扩展}

Scalable 1 set of electronic compass, 2 sets of NMEA or UBX standard GPS, CAN bus device (ESC), 2 I2C devices (smart battery, status light, optical flow smart camera, laser sensor, ultrasonic sensor, etc.)

### Technical specifications {#技术规格}

---

|  | **Hardware parameters** |
| :--- | :--- |
| Main processor Processor | STM32F427 |
| Coprocessor Failsafe co-processor | STM32F100 |
| **sensor** |  |
|accelerator Accelerometer 3 | LS303D\MPU6000 |
| Gyro 3 | L3GD20\MPU6000 |
| Compass 2 | LS303D |
| Barometer 2 | MS5611 |
| **interface** |  |
| Mavlink UART serial port | 2（With hardware flow control） |
| GPS UART serial port  | 2 |
| DEBUG UART serial port  | 1 |
| Remote signal input protocol | PPM/SBUS/DSM/DSM2 |
| RSSI input | PWM or 3.3 analog voltage|
| I2C | 2 |
| CAN Standard bus | 1 |
| ADC input | 3.3V X1 , 6.6V X1 |
| PWM output | Standard 8 PWM IO + 6 Programmable IOs|
|  |  |
| **Support models** |  |
|  | Plane / copter / helicopter / VTOL / rover etc.
|
| **Working environment and physical parameters** |  |
| PM working voltage | 4.5 ~ 5.5 V |
| USB voltage | 5.0 V +- 0.25v |
|Servo voltage | 4.8~5.4V |
| Operating temperature | -10 ~ 60°c |
| **Size** |  |
Long X Wide X High| 68\*44\*17 |
| Weight| 63g |





