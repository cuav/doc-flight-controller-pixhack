### Introduce {#介绍}

---

Pixhack is based on the Pixhawk hardware architecture platform designed by CUAV, and a 32-bit open source hardware flight control CUAV production, because the hardware main structure is the same with the pix, so it is fully compatible with 3DR APM firmware and Pix native firmware. PIXHACK optimizes the power chip on the basis of Pix original edition, cuts down unnecessary AUX6 interface, the interface makes adjustment and is optimized, change to front and rear insert line. The main highlights are the IMU's separation design, built-in small general-purpose shock absorbing structure, and the use of a CNC integrated milling process. The anti-jamming performance and stability are qualitatively improved. Pixhack has been through Cuav's one-year-long design. Numerous versions of optimization and testing have achieved stable and ideal results.

#### Cover all models {#覆盖全机型}

The Pixhack V2 is a drone control system built by CUAV that can run PX4 and APM environments.

Support includes: fixed-wing, copter \(3-8 rotors\), helicopters, VTOL drones, unmanned vehicles, unmanned boats.

#### Powerful processor {#强大处理器}

Based on STM32F427 \(180MHZ\) master and STM32F100 coprocessor.

#### Redundant design {#冗余设计}

* Built-in 2 IMU redundancy designs \(including 2 accelerometers, 2 gyros, 1 electronic compass, 1 digital barometer\)

* Supports 3 sets of power supply redundant switching

* The built-in sensor data fusion mechanism and failover mechanism in the software greatly reduce the chance of crashes caused by flight control.

#### Enrich expansion {#丰富扩展}

Scalable 1 set of electronic compass, 2 sets of NMEA or UBX standard GPS, CAN bus device \(ESC\), 2 I2C devices \(smart battery, status light, optical flow smart camera, laser sensor, ultrasonic sensor, etc.\)

#### Built-in shock absorber system {#内置减震系统 }

Separate design of sensor and main board, built-in high-performance shock absorption system, Able to adapt to a variety of severe environments
![](/assets/imu1.png)

### Technical specifications {#技术规格}

---

|  | Hardware parameters |
| :--- | :--- |
| Mian Processor | STM32F427 |
| Failsafe co-processor | STM32F100 |
| **sensor** |  |
| Accelerometer 3 | LS303D\MPU6000 |
| Gyro 3 | L3GD20\MPU6000 |
| Compass 2 | LS303D |
| Barometer 2 | MS5611 |
| I**nterface** |  |
| Mavlink UART | 2 \(with hardware flow control\) |
| GPS UART | 2 |
| DEBUG UART | 1 |
| Remote signal input protocol | PPM/SBUS/DSM/DSM2 |
| RSSI | PWM or 3.3 analog voltage |
| I2C | 2 |
| CAN Standard bus | 1 |
| ADC input | 3.3V X1 , 6.6V X1 |
| PWM output | Standard 8 PWM IO + 5 Programmable IOs |
|  |  |
| Support models |  |
|  |Plane / copter / helicopter / VTOL / rover etc.
|
| Working environment and physical parameters |  |
| PM working voltage | 4.5 ~ 5.5 V |
| USB voltage | 5.0 V +- 0.25v |
| Servo voltage | 4.8~5.4V |
| working temperature | -10 ~ 60°c |
| Size |  |
| Length x width x height | 68\*44\*17 |
| Weight | 63g |

### Interface cognition {#接口认识 }

---

![](/assets/pixhack port.png)

1.Main status light

2.Under State Lights

3.Safe unlock switch

4.DSM remote control signal + ADC6.6 interface

5.GPS+COMPASS interface

6.Digital interface

7.Bus expansion interface

8.DEBUG interface + GPS2 interface

9.POWER IV sensor interface

10.Micro USB interface

11.TF card interface

12.FMU STM32F4 restart button

13.IO STMF100 restart button



### Interface definition {#接口定义}

---

![](/assets/V33_legend.png)



