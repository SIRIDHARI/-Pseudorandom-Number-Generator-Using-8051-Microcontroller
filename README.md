# -Pseudorandom-Number-Generator-Using-8051-Microcontroller

Objective: 
Generating  a random number  using an 8051 microcontroller and displaying  the generated numbers on a 7
segment LED display. 
Abstract: 
The Aim of this project is to demonstrate the creation of pseudo-random numbers utilizing an 8051 
microcontroller, and the display of these generated numbers on a 7-segment LED display. 
Hardware / Software Requirements: 
• AT89C51 (8051 Microcontroller) 
• 8051 Programmer  
• Programming cable 
• 5V Power Supply 
• 16×2 Alphanumeric LCD 
• 2 Ceramic Capacitors – 33pF 
• 11.0592 MHz Crystal 
• Push Button – 3 
• Voltage Divider 
• Electrolytic Capacitor – 10μF, 16V 
• 10KΩ Resistor (1/4 watt) – 2 
• 330Ω Resistor (1/4 watt) – 2 
• POT – 10KΩ 
• 1KΩ X 8 Resistor Pack 
• Connecting Wires  
Working Principle: 
The random number generator circuit using an 8051 microcontroller relies on the microcontroller 
continuously incrementing a counter from 0 to 99 at high speed. When a specific button is pressed 
(connected to P3.0), the microcontroller captures the current counter value and displays it on a 16x2 LCD 
screen. This process results in the generation of a random number within the range 0 to 99. The LCD is 
connected to the microcontroller through Port 2, while another button (connected to P3.1) is used to reset the 
count. A reset circuit, an oscillator (11.0592 MHz crystal with two 33pF capacitors), and a potentiometer for 
LCD contrast control complete the circuit. Adjusting the potentiometer varies the LCD 
contrast or  brightness. 
 
Approach / Methodology / Programs: 
The project for the 8051 microcontroller-based random number generator utilizes an AT89C51 
microcontroller and an LCD to create a simple, pseudorandom number generator with a user-friendly 
interface. The code written in Keil μVision initializes the LCD, handles button presses, and generates 
random numbers from 0 to 99. The program continuously loops, displaying instructions to press a button to 
generate a random number, and then displays the generated number. When the "RST" button is pressed, the 
process restarts. This project is suitable for applications requiring random number generation and can serve 
as a basic example of microcontroller-based hardware interfacing and control structures. 
 
Code Overview: 
The code starts with including the necessary header files and defining some constants and pins. 
It defines various functions for LCD initialization, displaying characters, and converting integers to strings 
for display.In the main function, the program initializes the LCD, displays a welcome message, and waits for 
a button press.
Inside the infinite loop: 
• It displays a message to "Press the button." 
• It increments the i variable each time until a button press is detected. 
• It resets i to 0 when it reaches 100. 
• It displays the random number on the LCD and waits for the "RST" button to be pressed. 

Conclusion: 
The 8051 microcontroller-based random number generator project demonstrates the integration of hardware 
and software to achieve the generation of pseudorandom numbers within a specified range. By continuously 
incrementing a counter and capturing its value upon a button press, the project successfully generates 
random numbers from 0 to 99. The LCD interface provides a user-friendly experience, and the code, 
developed in Keil μVision, effectively manages the display and user input. This project serves as a practical 
example of microcontroller-based control structures and hardware interfacing and can be applied in various 
scenarios where random numbers are required, such as games and simulations. 
