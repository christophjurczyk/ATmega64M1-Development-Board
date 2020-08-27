# ATmega64M1-Development-Board (Arduino-Compatible)
<img src="/pcb_render/ATmega64M1_Dev_Board_top.png" alt="pcb" width="500px"/>

This projects brings an Arduino-compatible development board for the Atmel ATmega64M1 microcontroller. The ATmega64M1 is an 8-bit AVR RISC-based microcontroller and with the CAN capabilities widely used in the automotive industry.

The microcontroller has some additional features to the widely-used Arduino UNO:
- CAN interface
- DAC
- internal temperature sensor

With the help of ATmegaxxM1-C1 Arduino Core of thomasonw (https://github.com/thomasonw/ATmegaxxM1-C1) it is possible to work with the Arduino environment on this board. But you are also able to program the board directly via an ICSP and a dedicated programmer.


## Notes
### CAN Interface
The CAN interface can be handled by two CAN transceivers. You can choose between an isolated (ADM3053) and a non-isolated (MCP2562) CAN transceiver. If you are using the ADM3053, you have to equip the board with R6 and C12 to C15. C5 to C8 are mandatory for both configurations.

### Power Supply
You power the board via three different ways: USB, VIN (DC-Jack or pin header) or CAN interface (3: GND and 9: VCC). You can configure the power supply via the jumper JP2 and JP3 next to the DC-Jack. 
If you are using the CAN interface as power provision, you have to close the solder jumper SJ4 next to the CAN interface. **Caution:** If you are closing this jumper the grounds of the board and CAN interface are no more isolated to each other!

### Logic Level
You can run the controller with 5V or 3.3V. You can configure this via the jumper JP4 next to the DC-Jack.

## Stuff you'll need to buy, mount and reflow:
[bill of materials](billofmaterials.md)
