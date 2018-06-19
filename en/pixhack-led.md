## Pixhack LED status lights \(RGB three-color status lights\)

---

**Red and blue alternately flashing: **Initialize the sensor, please balance the autopilot board

**Blue flashing:** locked state (satisfaction with auto-steady mode unlockable condition), but GPS has not yet succeeded in 3D FIX. If the autopilot mode requires GPS positioning, it will Failed  to arm.

**Blue is always on:**The Autopilot  have been Arm but no GPS 

**Flashing green:** The Autopilot  have been Arm (and meets unlockable conditions), GPS is also 3D FIX locked.

**Fast flashing green: **Search for high-precision SBAS GPS satellites. The Autopilot  the locked state (and satisfies the unlockable condition), GPS is also 3D FIX.

**Green is always on - The buzzer emits a long beep: **The aircraft is unlocked and ready to take off

**Double flashing yellow light:** Unsuccessful arm (check Pre-Arm error message)

**Flashing yellow alone:** ​Failsafe activated

**Yellow blue flashing: - High - High - High (low buzzer) (dah-dah-dah-doh):** GPS fault or GPS failsafe  activation

**Red yellow flashing:** disable Kalman filter or inertial navigation (error)

**Purple yellow flashing:** barometer  fault 

**Solid red:** Hardware error. Usually no TF card (reinsert TF card or replace), MTD device or IMU sensor is detected. You can view boot directory information for BOOT.txt.

**Steady red, SOS sound:** SD card lost or SD card format error After the power is turned on, no lights are on. Firmware/firmware  lost; SD card lost or SD card malformed (ac3.4 or higher firmware)

