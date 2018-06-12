## Pixhack LED status lights \(RGB three-color status lights\)

---

**Red blue alternately flashes： **Initialize the sensor, please balance the Autopilot board

**Blue flashing：**Need GPS lock, the Autopilot board needs the mode of GPS signal, but GPS has not succeeded in positioning 3D FIX yet

**Blue always bright**：Armed has been unlocked, but no GPS lock

**Green flashing：**Locked state \(and meet the unlockable condition\), GPS also 3D FIX lock.

**Green flashes quickly：**Searched for high accuracy SBAS GPS satellites. Flight control lock status \(and meet the unlockable conditions\), GPS also 3D FIX.

** Green always bright --- The buzzer emits a long beep：**The plane is unlocked and ready to take off

**Yellow light Double flash:** Failed to unlock \(check Pre-Arm error message\)

**Flashing yellow alone: **Remote controller failure protection is activated

**Yellow Blue Flashing: **- High-High-High-Low \(buzzer\) \(dah-dah-dah-doh\): GPS malfunction or GPS fault protection activation

**Red Yellow Flashing: **Kalman filter or inertial navigation is disabled \(error\)

**Purple Yellow flashing: **Barometer error

**Red always bright: **Hardware error. Normally no TF card \(reinsert TF card or replacement\), MTD device, or IMU sensor is detected. You can view the boot directory information of BOOT.txt.

**Red always bright and SOS tone sound: **SD card lost or SD card format error After power-on, no light is turned on. Firmware/firmware is not lost; SD card is lost or SD card format is incorrect \(ac3.4 or higher firmware\)

