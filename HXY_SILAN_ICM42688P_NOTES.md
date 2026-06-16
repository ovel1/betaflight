Experimental Betaflight patch for HXY/Silan ICM42688P clone.

Tested on DAKEFPVF722-compatible STM32F722 target.
The chip reports WHO_AM_I = 0x6A at register 0x01.
Original Betaflight ICM42688P driver does not work because the register map differs from the TDK/InvenSense ICM42688P.

Build:
make configs
make DAKEFPVF722

Status:
Gyro/ACC detected and Setup model moves.
Sensor alignment may need to be configured in Betaflight.
Not flight-tested yet.
