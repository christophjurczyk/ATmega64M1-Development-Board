
#########################################################
# Bill of Materials 
# Per Unit in non-isolated can bus (MCP2562 config)

## Chips:
* 1x ATMEGA64M1					@ 14.00
* 1x FT232RL  IC4				@ 13.00
* 1x MCP2562  U1  				@ 6.00

## Capacitors: 
* 6x smd 1206 / 3216 polar 10uf tantulum    c1,c2,c3,c4,c5,c7		  @ 0.28  
* 6x smd 0805 / 2012 non-polar 100nf    c6,c8,c16,c17,c18,c19		@ 0.08
* 2x smd 0805 / 2012 non-polar 22pf   c9,c11			0.08

## Oscillators:
* 16mhz Q1  			@ 0.20

## Voltage Regulator:
* AMS1117 LM1117IMPX-3.3 15Vin 3.3Vout 800ma SOT223	IC1    	
* AMS1117 LM1117IMPX-5.0 15Vin 3.3Vout 800ma SOT223  IC2	   

## 0805 / 2012 Resistors:
* 6x 1k r1,r2,r4,r5, r8,r9		@ 0.10
* 1x 10k resistor    R3				
* 1x 120ohm resistor  r7

## 0302 Leds:
* 3x Green LED1,LED3,LED5
* 3x Orange LED2, LED4, LED6  			@ 0.04 x 6

## Misc: 
* 1x X1 micro USB
* 1x ISCP connector 3x2 pin header 	SV1
* 1x DC Jack - DCJ0202  J1
* 1x sw1 (reset)						@ 0.05
* 6x surface jumpers  sj1,sj2,sj3,sj4,sj5
* 1x fuse - f1 1206 / 3216 1.5A 6v 		@ 0.18

#################################################
# optional isolated can bus
smd 1206 / 3216 polar 10uf  C12,c15						
smd 0805 / 2012 non-polar 100uf  c13,14   
50 x 47k resistor r6  (optional for ADM3053)

#################################################
# Improved CAN terminator (replaces r7 120ohm) - coming soon!
2 x 60ohm  r7a r7b
1 x 4.7nf capacitor



----

