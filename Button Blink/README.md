# README for Button Blink

Ryan E. Drexel
	
	Created 24 September 2017
	Updated 09 October 2017

Embedded Systems- Dr. Tang and Mr. T.

Button blink is a C language program designed to run on five MSP430 microprocessors (listed below)
	MSP430G2553
	MSP430FR6989
	MSP430F5529
	MSP430FR2311
	MSP430FR5994
Button blink builds upon the polling system utilized in MSP430x Simple blink. See Simple Blink README for details.

	Button blink sets itself apart from single blink by polling for the push of a button rather 
	than the value of a timer. Every time the button is pressed, the polling check passes and the 
	LED values flip.