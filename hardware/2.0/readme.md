# OpentasticFan PCB

## Assembly Notes
- ESP32-SOLO-1 used on prototypes, for reduced JLCPCB assembly costs.
- All SMD parts are availible through LCSC/JLCPCB with "Economic PCB Assembly". If having JLCPCB do the SMD assembly, you will need to install/solder C5, U5, J1, J2, J3, J4, J6, J10
- If using a NTC thermistor instead of a DS18B20, change R15 to correct value for thermistor
- Recommend using JST XH headers for J3, J4, J6. They fit on this revision, but tightly.
- J5 doesn't need to be populated. It's currently unused.
- Install J1, J2, J10 so the screw terminals face out from the PCB with mating connector installed.

## Future Design changes
- Use ams1117 instead of switch mode regulator to reduce BOM costs/simplify.
- Replace .1" Headers with JST Connectors, for vibration resistance.
- Possibly replace DRV8874 with A4950E. This will likely result in needing to use a op-amp/current sense amplifier to monitor fan current?
