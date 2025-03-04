# Timer-in-DSM51
This assembly code is for the 8051 based microcontroller. It uses equ type commands to operate pins, e.g. LED = P1.7 and SOUND = P1.5. 


The code sets up the timers starting by setting the TMOD, TH0, TL0 registers and starts the timer using TR0. This is followed by a loop that waits until the timer finishes counting using the TF0 flag. The timer increments the seconds (R0), minutes (R1), and hours (R2) while displaying the updated time on the LCD screen in BCD format. The STOPER subroutine checks if the time is the same as a certain moment to change the LED state and sound. The program also asks the user for the start time and processes the input.
