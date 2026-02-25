## Experiment No: 5
ASTABLE MULTIVIBRATOR USING 555 TIMER Using Proteus
## Aim
To design and simulate an Astable Multivibrator using NE555 in Proteus Design Suite and observe the continuous square wave output.
## Apparatus Required
•	NE555 Timer IC
•	Resistor R1 = 10 kΩ
•	Resistor R2 = 100 kΩ
•	Capacitor C = 0.01 µF
•	DC Power Supply (5V or 9V)
•	CRO / Oscilloscope
•	Connecting wires
## Circuit Diagram
<img width="685" height="515" alt="Screenshot 2026-02-25 132155" src="https://github.com/user-attachments/assets/617a03ca-f7bd-4b46-95ab-b26e5549aa4e" />

Pin Configuration of 555 Timer:
•	Pin 1 → Ground
•	Pin 2 → Trigger
•	Pin 3 → Output
•	Pin 4 → Reset (Connected to Vcc)
•	Pin 5 → Control Voltage (Bypass with 0.01 µF capacitor optional)
•	Pin 6 → Threshold
•	Pin 7 → Discharge
•	Pin 8 → Vcc
## Connections:
•	R1 → Between Vcc and Pin 7
•	R2 → Between Pin 7 and Pins 2 & 6
•	C → Between Pins 2 & 6 and Ground
•	Output → Pin 3
## Theory
•	The NE555 timer is a widely used integrated circuit for generating precise time delays and oscillations. When operated in astable mode, it functions as a free-running oscillator that continuously produces a square wave without any external triggering signal. In this mode, a capacitor connected to the circuit charges through resistors R1 and R2 and discharges through R2 repeatedly. The internal voltage divider of the 555 timer creates two reference levels at 1/3 Vcc and 2/3 Vcc. 
•	When the capacitor voltage reaches 2/3 Vcc, the upper comparator resets the flip-flop and turns ON the discharge transistor, causing the capacitor to discharge. When the voltage falls to 1/3 Vcc, the lower comparator sets the flip-flop, turning OFF the discharge transistor and allowing the capacitor to charge again. This continuous charging and discharging process generates a square wave at the output (Pin 3) and an exponential waveform across the capacitor. The time period of oscillation is given by T=0.693(R1+2R2)CT = 0.693 (R1 + 2R2) CT=0.693(R1+2R2)C, and the frequency depends on the values of R1, R2, and C. Thus, the 555 timer in astable mode acts as a simple and reliable square wave generator used in clock circuits, LED flashers, and pulse generation applications.
## Procedure
1.	Open Proteus software.
2.	Select NE555 IC, resistors, capacitor, and CRO.
3.	Connect circuit in astable configuration.
4.	Apply 5V supply.
5.	Run simulation.
6.	Observe square wave output at Pin 3.
7.	Measure time period and frequency.
## Tabulation
| **S.No** | **R1 (kΩ)** | **R2 (kΩ)** | **C (µF)** | **Theoretical Frequency (Hz)** | **Practical Frequency (Hz)** |
| -------- | ----------- | ----------- | ---------- | ------------------------------ | ---------------------------- |
| 1        | 10          | 500         | 0.1        | 14.25                          | 14.25                        |

## Waveforms
<img width="692" height="461" alt="image" src="https://github.com/user-attachments/assets/b3eb9549-44a2-465c-97ea-ec768bda02be" />

•	Output (Pin 3) → Square wave
•	Capacitor voltage → Exponential charging & discharging waveform
## Result
The Astable Multivibrator using NE555 Timer IC was successfully designed and simulated in Proteus.
A continuous square wave output was obtained.
The practical frequency closely matches the theoretical frequency.
## Conclusion
•	The 555 timer works as a free-running oscillator in astable mode.
•	Frequency depends on R1, R2, and C values.
•	Increasing R or C decreases frequency.
•	Used in clock generation, LED flashing, and tone generation.
## Viva Questions

1. What are the operating modes of 555 timer?
The 555 timer operates in three different modes namely monostable mode, astable mode and bistable mode, depending on the external components connected to it.

2. What are the threshold levels in astable mode?
In astable mode of the 555 timer, the capacitor voltage continuously varies between one-third of the supply voltage and two-thirds of the supply voltage.

3. Write the frequency formula.
The frequency of oscillation in astable mode of the 555 timer is given by
  f = 1.44/(R1+2R2)C

5. What is duty cycle?
Duty cycle is defined as the ratio of the time for which the output remains HIGH to the total time period of the waveform and is usually expressed in percentage.

6. What happens if R2 increases?
When the value of resistor R2 is increased, the charging and discharging time of the capacitor increases, which results in an increase in time period and a decrease in frequency.
