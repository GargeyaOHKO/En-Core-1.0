Here’s a summarized **GitHub README** for your buck converter design project based on the document:

---

# **Buck Converter Design: En-Core 1.0**

## **Introduction**
This project involves designing a non-isolated buck converter that steps down a 24V input to a 5V output with an efficiency of at least 90%. The buck converter is essential in many power conversion applications, such as power supplies and electric vehicles. 

### **Key Specifications:**
- **Input Voltage (Vin):** 24V (±2% tolerance)
- **Output Voltage (Vout):** 5V (±0.01V)
- **Input Current:** 1A max
- **Efficiency:** ≥ 90%
- **Form Factor:** Max PCB size of 10 cm x 5 cm

---

## **Theoretical Background**
A buck converter reduces the input voltage to a lower output voltage by switching a MOSFET on and off. The energy is stored in an inductor and smoothed out by a capacitor. The main components are:
- **Schottky Diode (1N5817):** Minimizes losses.
- **PWM Source (NE555 Timer):** Generates the switching signal.
- **Inductor and Capacitor:** For energy storage and output voltage smoothing.

### **Efficiency Calculation:**
Efficiency depends on losses in the MOSFET (switching and conduction losses), inductor, and other components.

---

## **Simulation and Testing**

The circuit was simulated to verify the design, focusing on:
- Input voltage (24V DC)
- PWM signal generated by the NE555 (duty cycle 20.8%)
- Output voltage (5V with 0.02V ripple)

![6316340018767052681](https://github.com/user-attachments/assets/e45e4156-eb1f-41fd-a5f7-5a55e0141f44)


**Simulation Graphs:**
- **Green:** 24V input voltage
- **Blue:** PWM signal from the NE555 timer
- **Red:** 5V output DC voltage

![6316340018767052683](https://github.com/user-attachments/assets/14bab19d-61ed-4403-afee-09918fa89163)


---

## **Schematic and PCB Design**
- **Schematic:** Designed using KiCad, featuring a PWM generator (NE555), MOSFET, Schottky diode, inductor, and output capacitor.
- **PCB Design:** A dual-layer design to ensure proper thermal management, minimized noise, and correct trace width for current handling.

![Schematic](https://github.com/user-attachments/assets/7cce3dc8-1727-4691-8b37-dde8df1e5275)

![Kicad pcb](https://github.com/user-attachments/assets/3b5c19bc-508d-41c2-8081-fe6bc3845eb5)

![Kicad pcb2](https://github.com/user-attachments/assets/ae1f18c5-6745-4b51-b6ae-48633e165ca7)

![6316340018767052651](https://github.com/user-attachments/assets/18c0d9bc-3374-4f61-806f-785a8bb9ff37)

---

## **Conclusion**
The buck converter successfully steps down 24V to 5V with over 90% efficiency, meeting all design and dimensional constraints.

---

## **Project Links**
- [GitHub Repository](https://github.com/GargeyaOHKO/En-Core-1.0)
- [YouTube Simulation Video](https://youtu.be/STvGI6kvZm8)

---



