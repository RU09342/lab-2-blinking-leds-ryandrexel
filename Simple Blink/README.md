# README for Simple Blink

Ryan E. Drexel
	
	Created 24 September 2017
	Updated 03 October 2017

Embedded Systems- Dr. Tang and Mr. T.

Simple blink is a C language program designed to run on five MSP430 microprocessors (listed below)
	MSP430G2553
	MSP430FR6989
	MSP430F5529
	MSP430FR2311
	MSP430FR5994
Simple blink is incredibly simple; it uses an unsigned integer to count up to a value FFFFh (65535d, 111111111111111b)
Each time the counter reaches this value, it resets to 0 and inverts the state of the LED.

The program uses a while (1) loop to run endlessly, and uses at technique called polling to check the value of the counter
	
	The polling technique referes to code that checks an entity periodically in order to trigger an event
	when that particular entity satisfies a condition. This program uses an "if" statement to check if the
	counter is equal to the value FFFFh. This check occurs each time the program repeats the while loop.