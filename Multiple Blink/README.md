# README for Multiple Blink

Ryan E. Drexel
	
	Created 24 September 2017
	Updated 03 October 2017

Embedded Systems- Dr. Tang and Mr. T.

Multiple blink is a C language program designed to run on five MSP430 microprocessors (listed below)
	MSP430G2553
	MSP430FR6989
	MSP430F5529
	MSP430FR2311
	MSP430FR5994
Multi blink builds upon the polling system utilized in MSP430x Simple blink. See Simple Blink README for details.

	Multi blink sets itself apart from single blink by using the same counter to manipulate
	two different LEDs at two different rates. One LED changes state at counter = FFFFh (65535d, 111111111111111b),
	while the other LED changes state at twice the rate.
		This second LED changes state at counter = FFFFh AND counter = 8000h (32767d, 011111111111111b)