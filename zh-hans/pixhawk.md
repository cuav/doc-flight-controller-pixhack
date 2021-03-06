### 介绍 {#介绍}

---

Pixhawk是世界上最出名的开源飞控硬件厂商3DR推出的开源飞控。Pixhawk作为开源硬件且具有强大的功能，可靠的性能等到了广大用户的青睐。其硬件的开源使不少的硬件厂商加入了制造pixhawk的行列，cuav作为国内知名的开源飞控的厂商，其按照pixhawk原版的设计，采用相同的硬件设计及全进口芯片，使其生产出来的pixhawk具有相当高的稳定性。

#### 覆盖全机型 {#覆盖全机型}

Pixhawk是一款的无人机控制系统，可运行 PX4 及 APM 环境。

支持包括：固定翼、多旋翼（3-8 旋翼）、直升机、垂直起降无人机 VTOL、无人车、无人船。

#### 强大处理器 {#强大处理器}

基于 STM32F427（180MHZ）主控及 STM32F100 协处理器。

#### 冗余设计 {#冗余设计}

* 内置 2组 IMU 冗余设计（包括 2 组加速计、2组陀螺仪、1组电子罗盘、1组数字气压计）

* 支持 3 组电源供电冗余切换

* 软件内建传感器数据融合机制及故障切换机制，将由飞控引起的坠机几率大大降低。

#### 丰富扩展 {#丰富扩展}

可扩展 1 组电子罗盘、2 组 NMEA 或者 UBX 标准 GPS、CAN 总线设备（电调）、2 路 I2C 设备（智能电池、状态灯、光流智能相机、激光传感器、超声波传感器等）

### 技术规格 {#技术规格}

---

|  | **硬件参数** |
| :--- | :--- |
| 主处理器Processor | STM32F427 |
| 协处理器Failsafe co-processor | STM32F100 |
| **传感器** |  |
| 加速器Accelerometer 3 | LS303D\MPU6000 |
| 陀螺仪Gyro 3 | L3GD20\MPU6000 |
| 电子罗盘Compass 2 | LS303D |
| 气压计Barometer 2 | MS5611 |
| **接口** |  |
| Mavlink UART串口 | 2（带硬件流控） |
| GPS UART串口 | 2 |
| DEBUG UART串口 | 1 |
| 遥控器信号输入协议 | PPM/SBUS/DSM/DSM2 |
| RSSI输入 | PWM或3.3模拟电压 |
| I2C | 2 |
| CAN标准总线 | 1 |
| ADC输入 | 3.3V X1 , 6.6V X1 |
| PWM输出 | 标准8 PWM IO + 6个可编程IO |
|  |  |
| **支持机型** |  |
|  | 固定翼/3-8旋翼/直升机/VTOL垂直起降/无人机/无人船 |
| **工作环境及物理参数** |  |
| PM工作电压 | 4.5 ~ 5.5 V |
| USB电压 | 5.0 V +- 0.25v |
| Servo电压 | 4.8~5.4V |
| 工作温度 | -10 ~ 60°c |
| **尺寸** |  |
| 长X宽X高 | 68\*44\*17 |
| 重量 | 63g |





