# OpentasticFan PCB 3.0

## Updates from 2.0
- Uses ESP32-S3 instead of classic ESP32 (U5)
- USB for programming intergrated (J9, R6, R8, D1)
- Uses DRV8874PWR(U1, U2) for both motor controls. Combined with the better ADC of the ESP32-S3 gives accurate current measurement.
- AMS1117(U3) instead of switch mode regulator for power supply to reduce BOM cost
- Changed from Dallas DS18B20 to NTC thermistor(TH1) for air temperature for both the reduced cost, and due to the flaky support in ESPHome
- Added i2c pullup resistors (R1, R2)

## Assembly Notes
- ESP32-S3-WROOM-1 used, due to poor ADC on the classic ESP32. It is not availible for JLCPCB "Economic PCB Assembly" and will need to be hand soldered.
- Most SMD parts are availible through LCSC/JLCPCB with "Economic PCB Assembly". If having JLCPCB do the SMD assembly, you will need to install/solder C5, J1, J2, J3, J4, J6, J7, J8, U5
- J5 doesn't need to be populated. It's currently unused.
- Install J1, J2, so the screw terminals face out from the PCB with mating connector installed.


