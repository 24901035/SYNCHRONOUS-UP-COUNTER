### SYNCHRONOUS-UP-COUNTER

**AIM:**

To implement 4 bit synchronous up counter and validate functionality.

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 bit synchronous UP Counter**

If we enable each J-K flip-flop to toggle based on whether or not all preceding flip-flop outputs (Q) are “high,” we can obtain the same counting sequence as the asynchronous circuit without the ripple effect, since each flip-flop in this circuit will be clocked at exactly the same time:

![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/d5db3fa0-e413-404c-b80e-b2f39d82e7e8)


![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/52cb61eb-d04b-442d-810c-31185a68410b)

Each flip-flop in this circuit will be clocked at exactly the same time.
The result is a four-bit synchronous “up” counter. Each of the higher-order flip-flops are made ready to toggle (both J and K inputs “high”) if the Q outputs of all previous flip-flops are “high.”
Otherwise, the J and K inputs for that flip-flop will both be “low,” placing it into the “latch” mode where it will maintain its present output state at the next clock pulse.
Since the first (LSB) flip-flop needs to toggle at every clock pulse, its J and K inputs are connected to Vcc or Vdd, where they will be “high” all the time.
The next flip-flop need only “recognize” that the first flip-flop’s Q output is high to be made ready to toggle, so no AND gate is needed.
However, the remaining flip-flops should be made ready to toggle only when all lower-order output bits are “high,” thus the need for AND gates.

**Procedure**

/* write all the steps invloved */
![Screenshot 2025-01-06 115644](https://github.com/user-attachments/assets/60d47717-4140-46d7-8be9-1062a6eb3906)


**PROGRAM**

/* Program for flipflops and verify its truth table in quartus using Verilog programming. 

Developed by: RegisterNumber:
*/
![Screenshot 2025-01-06 115657](https://github.com/user-attachments/assets/b1939c5f-1b62-48b2-b2dc-64df79bf1b5f)


**RTL LOGIC UP COUNTER**
![Screenshot 2025-01-06 115709](https://github.com/user-attachments/assets/25d4bd46-2a55-4bc0-8ba3-a3ac5f50febe)

**TIMING DIAGRAM FOR IP COUNTER**
![Screenshot 2025-01-06 115721](https://github.com/user-attachments/assets/746b33d9-b755-424e-a575-6462e6b9fe06)

**TRUTH TABLE**
![Screenshot 2025-01-06 115733](https://github.com/user-attachments/assets/31da685b-5e31-4572-a6f7-b430d7a121f0)

**RESULTS**
Thus the given 4 bit synchronous up counter are implimented using and validate functionality are verified using verilog programming.
