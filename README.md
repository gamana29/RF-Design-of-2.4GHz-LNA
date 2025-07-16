# RF-Design-of-2.4GHz-LNA
Designing a Radio Frequency Design for 2.4GHZ Low Noise Amplifier using Cadence Virtuoso.

Technology used - 45nm CMOS Technology

Goal of project - To optimiza LNA's performancewith low noise figure, adequate gain, and minimal power dissipation.

Low Noise Amplifiers ensures efficient reception of weak signals. To design an LNA we need to balance between high gain, low noise figure(NF) and low power consumption.

Noise Figure - Quantifies the noise added to the I/P signal during amplification.

To analyze amplifier various simulation techiniques like S-parameter analysis and P-noise analysis is done, to asses it's performance in the desired frequency range(2.4GHz ISM band).

The 2.4Ghz frequency band is widely used for technologies such as Wi-Fi,Bluetooth and Zigbee, it also emphasizes the importance of designing high-performance LNAs.

S-Parameter Analysis
S-parameter analysis was used to find the amplifier's gain, input/output reflection, and reverse transmission characteristics within a frequency span of 1 GHz to 5 GHz. Sweep was taken in automatic mode with frequency increment of about 80 MHz. The analysis revealed important parameters including:

S11 (Input Reflection): < -10 dB, which is good input matching.
S21 (Gain): 15–18 dB at 2.4 GHz, which is sufficient amplification.
S22 (Output Reflection): < -10 dB, which verifies output matching.
S12 (Reverse Isolation): < -30 dB, which is excellent isolation.


Periodic Noise (Pnoise) Simulation
Large signal noise performance was evaluated through Pnoise simulation. This simulation took into account the input noise, output noise, and noise transfer function in periodic steady-state operation. This analysis is particularly valuable for the examination of circuits working with time-varying signals, like RF LNAs.

Total Power Dissipation (Ptotal):
The total power dissipation is determined by the supply voltage (VDD = 3.3 V) and the total 
current consumed by the LNA. For a total current of 10 mA, the total power dissipation is:

Ptotal = 3.3V × 10mA = 33mW

---------
Result

<img width="695" height="479" alt="image" src="https://github.com/user-attachments/assets/d774407a-184a-4904-95f3-b71af55e8d3d" />
•	fig 1 : Comparing output noise and input
(pnoise – periodic noise)


<img width="669" height="454" alt="image" src="https://github.com/user-attachments/assets/78d24d30-72e8-4a36-b600-2ba3981a9735" />
•	fig2 : Noise Figure for NF(dB10) and NF mag (dB10)


<img width="663" height="681" alt="image" src="https://github.com/user-attachments/assets/e0b0e81b-bbb0-4572-a327-4d676c4c4e79" />
The simulation is performing a S-parameter analysis over a frequency range of 1 GHz to 5 GHz.
The sweep is done in steps of 80 MHz, meaning it checks circuit behavior at many points between 1 and 5 GHz.
Each frequency point (e.g., 1.00 GHz, 1.08 GHz, …) shows the S-parameter results, typically S11, S21, S12, S22, etc.





