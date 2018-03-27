
---

### Introduce {#介绍}

---

---

![](/assets/pixhackv31.png)

#### Cover all models {#覆盖全机型}

The Pixhack V3 is a new drone control system created by CUAV that can run PX4 and APM environments.

Support includes: fixed-wing, multi-rotors \(3-8 rotors\), helicopters, VTOL drones, unmanned vehicles, unmanned boats.

#### Powerful processor {#强大处理器}

Based on STM32F427 \(180MHZ\) master and STM32F100 coprocessor.

#### Redundant design {#冗余设计}

* Built-in 3 IMU Redundant Designs \(includes 3 accelerometers, 3 sets of gyroscopes, 2 sets of electronic compass, 2 sets of digital barometers\)

* Supports 3 sets of power supply redundant switching

* The built-in sensor data fusion mechanism and failover mechanism in the software greatly reduce the chance of crashes caused by flight control.

####  Enrich extension {#丰富扩展}

Scalable 1 set of electronic compass, 1 smart battery, 2 sets of NMEA or UBX standard GPS, CAN bus device \(ESC\), 2 I2C devices \(smart battery, status light, optical flow smart camera, laser sensor, ultrasonic sensor, etc.

#### Built-in shock absorber system {#内置减震系统}

Separate design of sensor and main board, built-in high-performance shock absorption system, a variety of severe model environment, better adaptability

#### Built-in IMU temperature automatic compensation system {#内置-imu-温度自动补偿系统}

Pixhack V3 has recently designed a digital temperature control system to keep the sensor in a constant temperature environment for better sensor performance consistency in order to adapt to a more severe low temperature environment.

### Technical specifications {#技术规格}

---

|  | **硬件参数** |
| :--- | :--- |
| 主处理器Processor | STM32F427 |
| 协处理器Failsafe co-processor | STM32F100 |
| **传感器** |  |
| 加速器Accelerometer 3 | LS303D\MPU6000\MPU9250 |
| 陀螺仪Gyro 3 | L3GD20\MPU6000\MPU9250 |
| 电子罗盘Compass 2 | LS303D\MPU9250 |
| 气压计Barometer 2 | MS5611 X2 |
| **接口** |  |
| Mavlink UART串口 | 2（带硬件流控） |
| GPS UART串口 | 2 |
| DEBUG UART串口 | 1 |
| 遥控器信号输入协议 | PPM/SBUS/DSM/DSM2 |
| RSSI输入 | PWM或3.3模拟电压 |
| I2C | 2 |
| CAN标准总线 | 1 |
| ADC输入 | 3.3V X1 , 6.6V X1 |
| PWM输出 | 标准8 PWM IO + 5个可编程IO |
|  |  |
| **支持机型** |  |
|  | 固定翼/3-8旋翼/直升机/VTOL垂直起降/无人机/无人船 |
| **工作环境及物理参数** |  |
| PM工作电压 | 4.5 ~ 5.5 V |
| USB电压 | 5.0 V +- 0.25v |
| Servo电压 | 4.8~5.4V |
| 工作温度 | -20 ~ 60°c |
| **尺寸** |  |
| 长X宽X高 | 68\*44\*17 |
| 重量 | 63g |

### 接口认识 {#接口认识}

---

![](/assets/pixhack port.png)

1. 主要状态灯
2. 底层状态灯
3. 安全解锁开关
4. DSM遥控信号+ADC6.6接口
5. GPS+COMPASS接口
6. 数传接口
7. 总线扩展接口
8. DEBUG接口+GPS2接口
9. POWER IV传感器接口
10. micro USB接口
11. TF卡接口
12. FMU STM32F4重启按键
13. IO STMF100 重启按键

    ### 接口定义 {#接口定义}

    ---

    ![](/assets/V33_legend.png)



