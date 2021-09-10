<h1>
  Basics-of-UART-Protocol
</h1>

<h2>
  Introduction
</h2>
One of the protocols used today for troubleshooting is the Universal Asynchronous Reciever Transmitter Protocol (UART). Based on this protocol, the standards RS-232, RS-422, RS-485, etc., are defined in the form of full-duplex or half-duplex. This protocol does not have a pulse clock, and the origin and destination transmit data to each other according to one baud rate or a contract that has certain values(3200, 4800, 9600, 3840, 57600, 115200, 256000, 1000000, 2000000) that of course, the transmitter chip must supports these speeds.
This protocol can be placed between two microcontrollers or a microcontroller and a computer, but to connect it to a computer, you need a converter called usb to serial or usb to rs-232.
In this project, we are going to establish a connection between the computer and the ARM microcontroller using FT232RL chip.

<h2>
  Implementation
</h2>
The library is based on ARM Programming Language and written in Keil uVision, a window-based software development platform for ARM-based microcontrollers. 
The microcontroller used is STM32F103 - Arm Cortex-M3 Microcontrollers.
There are multiple libraries for writing the program to implement on ARM microcontrollers, and generally, I would prefer to use the HAL library for STM32 ARM Cortex.
