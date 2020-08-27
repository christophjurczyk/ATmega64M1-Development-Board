
#########################################################
# Bill of Materials (Thanks to @elasticdotventures)
# Per Unit in non-isolated can bus (MCP2562 config)

## Chips:
* 1x ATMEGA64M1 IC11
* 1x FT232RL  IC4
* 1x MCP2562  U1

## Capacitors: 
* 6x smd 1206 / 3216 polar 10uf tantulum    c1,c2,c3,c4,c5,c7
* 6x smd 0805 / 2012 non-polar 100nf    c6,c8,c16,c17,c18,c19
* 2x smd 0805 / 2012 non-polar 22pf   c9,c11

## Oscillators:
* 16mhz Q1

## Voltage Regulator:
* AMS1117 LM1117IMPX-3.3 15Vin 3.3Vout 800ma SOT223	IC1    	
* AMS1117 LM1117IMPX-5.0 15Vin 3.3Vout 800ma SOT223  IC2	   

## 0805 / 2012 Resistors:
* 6x 1k r1,r2,r4,r5, r8,r9
* 1x 10k resistor    R3				
* 1x 120ohm resistor  r7

## 0805 Leds:
* 6x color your choice

## Misc: 
* 1x X1 micro USB
* 1x ISCP connector 3x2 pin header 	SV1
* 1x DC Jack - DCJ0202  J1
* 1x sw1 (reset)
* 6x surface jumpers  sj1,sj2,sj3,sj4,sj5
* 1x smd fuse 1206 f1

#################################################
# optional isolated can bus ADM3053
2x smd 1206 / 3216 polar 10uf  C12,c15						
2x smd 0805 / 2012 non-polar 100uf  c13,14   
1x 47k 0805 resistor r6

#################################################
# Improved CAN terminator (replaces r7 120ohm) - coming soon!
2 x 60ohm  r7a r7b
1 x 4.7nf capacitor



----

