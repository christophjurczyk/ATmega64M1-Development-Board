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

# Bill of Materials (Thanks to @elasticdotventures)
Per Unit in non-isolated can bus (MCP2562 config)

### Chips:
* 1x ATMEGA64M1 IC11
* 1x FT232RL  IC4
* 1x MCP2562  U1

### Capacitors: 
* 6x smd 1206 / 3216 polar 10uf tantulum    c1,c2,c3,c4,c5,c7
* 6x smd 0805 / 2012 non-polar 100nf    c6,c8,c16,c17,c18,c19
* 2x smd 0805 / 2012 non-polar 22pf   c9,c11

### Oscillators:
* 16mhz Q1

### Voltage Regulator:
* AMS1117 LM1117IMPX-3.3 15Vin 3.3Vout 800ma SOT223	IC1    	
* AMS1117 LM1117IMPX-5.0 15Vin 3.3Vout 800ma SOT223  IC2	   

### 0805 / 2012 Resistors:
* 6x 1k r1,r2,r4,r5, r8,r9
* 1x 10k resistor    R3				
* 1x 120ohm resistor  r7

### 0805 Leds:
* 6x color your choice

### Misc: 
* 1x X1 micro USB
* 1x ISCP connector 3x2 pin header 	SV1
* 1x DC Jack - DCJ0202  J1
* 1x sw1 (reset)
* 6x surface jumpers  sj1,sj2,sj3,sj4,sj5
* 1x smd fuse 1206 f1

### optional isolated can bus ADM3053
2x smd 1206 / 3216 polar 10uf  C12,c15						
2x smd 0805 / 2012 non-polar 100uf  c13,14   
1x 47k 0805 resistor r6

### Improved CAN terminator (replaces r7 120ohm) - coming soon!
2 x 60ohm  r7a r7b
1 x 4.7nf capacitor
