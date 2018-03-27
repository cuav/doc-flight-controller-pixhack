### Introduce {#介绍}

---

Pixhack is based on the Pixhawk hardware architecture platform designed by CUAV, and a 32-bit open source hardware flight control CUAV production, because the hardware main structure is the same with the pix, so it is fully compatible with 3DR APM firmware and Pix native firmware. PIXHACK optimizes the power chip on the basis of Pix original edition, cuts down unnecessary AUX6 interface, the interface makes adjustment and is optimized, change to front and rear insert line. The main highlights are the IMU's separation design, built-in small general-purpose shock absorbing structure, and the use of a CNC integrated milling process. The anti-jamming performance and stability are qualitatively improved. Pixhack has been through Cuav's one-year-long design. Numerous versions of optimization and testing have achieved stable and ideal results.

#### Cover all models {#覆盖全机型}

Pixhack V2是一款的无人机控制系统，由CUAV全新打造，可运行 PX4 及 APM 环境。

支持包括：固定翼、多旋翼（3-8 旋翼）、直升机、垂直起降无人机 VTOL、无人车、无人船。

#### 强大处理器 {#强大处理器}

基于 STM32F427（180MHZ）主控及 STM32F100 协处理器。

#### 冗余设计 {#冗余设计}

* 内置 2组 IMU 冗余设计（包括 2 组加速计、2组陀螺仪、1组电子罗盘、1组数字气压计）

* 支持 3 组电源供电冗余切换

* 软件内建传感器数据融合机制及故障切换机制，将由飞控引起的坠机几率大大降低。

#### 丰富扩展 {#丰富扩展}

可扩展 1 组电子罗盘、2 组 NMEA 或者 UBX 标准 GPS、CAN 总线设备（电调）、2 路 I2C 设备（智能电池、状态灯、光流智能相机、激光传感器、超声波传感器等）

#### 内置减震系统 {#内置减震系统}

传感器与主板分离设计，内置高性能减震系统,各种严峻机型环境，适应性更强

![](/assets/imu1.png)

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
| PWM输出 | 标准8 PWM IO + 5个可编程IO |
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



