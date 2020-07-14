# Real Time Audio to Frequency Spectrum Transformation on Atmega32 Microcontroller

A project to demonstrate frequency spectrum visualization from real time audio via time domain to frequency domain conversion on Atmega32 microcontroller.  
This repo contains an Atmel Studio project with software codes to simulate a real time audio to frequency spectrum transformation on Atmega32 Microcontroller using Discrete Fourier Transform (DFT).  
This project was implemented as hardware project of [Microprocessors and Microcontrollers Sessional course (CSE-316)](https://github.com/Subangkar/Microcontroller-CSE-316-BUET) of Department of CSE, BUET in Level-3, Term-1
  
**Project Requirements:**  
- Hardware:
    - Electret Microphone Breakout (https://www.sparkfun.com/products/12758)
    - Audio Jack (to feed audio input directly from phone)
    - OP-AMP LM358
    - Atmega32
    - Bi-color Dot Matrix of shape 8x8 (x2)
    - LCD (used for debug purpose only)
    - Breadboard
    - 5v Power Source
- Software:
    - Atmel Studio
    - AVR-GCC Compiler
    - [Extreme Burner](https://extreme-burner-avr.software.informer.com/)
    
**Input:**  
- Input Frequency: 200-4kHz
- Sampling Frequency: 8kHz
- DFT mode: 32-Point DFT
- PIN spec of Atmega32:
    - ADC0 - Mic input
    - ADC1 - Audio Jack input
  
**Output:**  
Amplitude plotted on two Dot Matrices consist of uniformly distributed 16 frequency bins over 0-4kHz.  
Each bin has amplitude height of 8. Lower amplitude frequencies cause dot matrix to have green bars on corresponding bin columns while red is for the higher amplitudes.  
  
  
**Project Contributors:**  
- [Subangkar Karmaker Shanto](https://github.com/Subangkar) (subangkar.karmaker@gmail.com)  
- Zahin Wahab (zahinwahab@gmail.com) 

**Project Supervisors:**  
- Dr. A.B.M Alim Al Islam  
Associate Professor, Department of CSE, BUET
- Abdus Salam Azad  
Assistant Professor, Department of CSE, BUET  
- Ahamed Al Nahian  
Lecturer, Department of CSE, BUET
  
  
**Demonstration Video:** [YouTube](https://www.youtube.com/watch?v=k5cmo2vL5w4) or [Local](/Demonstration.mp4)
  
  
**Credits & References:**  
- Audio Used: https://www.youtube.com/watch?v=qNf9nzvnd1k
- 32-Point Integer DFT: https://blog.vinu.co.in/2012/05/implementing-discrete-fourier-transform.html
- Mathematical Background of Sampling Rate Selection:
    - https://people.ece.cornell.edu/land/courses/ece4760/FinalProjects/f2012/ajw89_bwj8/ajw89_bwj8/index.html
    - https://www.waitingforfriday.com/?p=325
    
**More related codes/design on this [repo](https://github.com/Subangkar/Microcontroller-CSE-316-BUET/tree/master/AudioSpecViz)**.
