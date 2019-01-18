# Breakout board for ICM-20948 with i2c

This repository contains a breakout board for the 9-DOF Inertial Measurement Unit (IMU) from TDK, ICM-20948 ([data sheet](https://www.invensense.com/wp-content/uploads/2016/06/DS-000189-ICM-20948-v1.3.pdf)). The i2c communication pins and the interrupt pin has external connection. The board is designed for 3.3v power supply, as the IMU requires 1.8v IO-levels there is a voltage level translator that translate IO-levels to the supply voltage. As the voltage level translator contains internal pull up resistors, there is no need to have extra pull up resistors on the IO-lines.

### Note
This board has no yet been produced and tested yet. As this is one of my first designs I welcome any comments or suggestions that you might have.

I have some clearance issue in Eagle with the footprint of the ICM-20948. If someone knows how to fix this, please let me know.

## Bill of Material

- U1: NCP563SQ18T1G, 1.8v voltage regulator ([data sheet](https://www.onsemi.com/pub/Collateral/NCP562-D.PDF))
- U2: NTS0104, voltage level translator, ([data sheet](https://www.nxp.com/docs/en/data-sheet/NTS0104.pdf))
- U3: ICM-20948, IMU, ([data sheet](http://www.invensense.com/wp-content/uploads/2016/06/DS-000189-ICM-20948-v1.3.pdf))
- C1, C2, C3: Capacitor 0402, 0.1uF
- C4, C5: Capacitor 0402, 1.0uF
- R1: Resistor 0402, 10kOhm
- J1, J2: 3-pin 0.1'/2.54mm connectors

## Repository Contents
- /Hardware - Eagle design files (.brd, .sch)

## License Information
The hardware is released under [Creative Commons Share-alike 3.0](http://creativecommons.org/licenses/by-sa/3.0/).  
