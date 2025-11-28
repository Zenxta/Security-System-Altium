# Alarm Security System 

This project develops a low-cost and reliable Security Alarm System utilizing a Bipolar Junction Transistor (BJT) and a Silicon-Controlled Rectifier (SCR).
The system's core mechanism detects unauthorized access by sensing interruptions in an Infrared (IR) beam. The critical feature is the use of the SCR, which ensures a latching mechanism — the alarm remains active until manually reset even if the triggering event is brief.

### **Key Features**

* **Sensing Mechanism:** Uses an invisible **IR LED** and **IR Photodiode** setup, providing an advantage over visible light systems.
* **Persistent Alert:** A **TYN612 SCR** provides the critical latching function. Once triggered, the alarm remains ON until manually reset ensuring brief intrusions are not missed.
* **Adjustable Sensitivity:** A **$100\ k\Omega$ Potentiometer** allows the user to fine-tune the circuit's sensitivity for different environmental conditions.
* **Power & Enclosure:** Powered by rechargeable **18650 Li-ion cells** with a **TP4056 charging module** (Type-C) and protected by a custom 3D-printed enclosure.

---

| Component | Type | Quantity | Description |
| :--- | :--- | :--- | :--- |
| **Transistor** | BC547 (BJT) | 1 | Amplifies the weak photodiode signal to trigger SCR |
| **Latching Device** | TYN612 (SCR) | 1 | Maintains alarm status until power is interrupted |
| **Sensing Pair** | IR LED, IR Diode | 1, 1 | Creates and detects the invisible security beam |
| **Adjuster** | Potentiometer ($100\ k\Omega$) | 1 | Fine-tunes the tripping point/sensitivity |
| **Output** | Buzzer | 1 | Audible alert signal |
| **Power** | Li-ion Cell (18650) | 2 | Rechargeable power source for the circuit |
| **Charging** | TP4056 Module | 1 | Facilitates Type-C charging for the cells within the enclosure |

### **Project Files**

All files required for manufacturing and design review are included in the repository.

* **Schematic:** `Security_Alarm_System.SchDoc`
* **PCB Layout:** `Security_Alarm_System.PcbDoc`
* **Gerber Files:** `Gerber_Files.zip`

---

### **Design Files & Visualization**

The Schematic and PCB Layout were designed using Altium Designer software

#### **Schematic Diagram**

<img width="1200" height="800" alt="Schematic Diagram of the BJT-SCR Security Alarm Circuit" src="https://github.com/Zenxta/Security-System-Altium/blob/main/Schematic%201.jpeg?raw=true" />

<img width="1200" height="800" alt="Schematic Diagram of the BJT-SCR Security Alarm Circuit" src="https://github.com/Zenxta/Security-System-Altium/blob/main/Schematic%202.jpeg?raw=true" />

#### **PCB Layout**

<img width="1200" height="800" alt="PCB Layout for the BJT-SCR Security Alarm" src="https://github.com/Zenxta/Security-System-Altium/blob/main/PCB%20Board%201.jpeg?raw=true" />

<img width="1200" height="800" alt="PCB Layout for the BJT-SCR Security Alarm" src="https://github.com/Zenxta/Security-System-Altium/blob/main/PCB%20Board%202.jpeg?raw=true" />

#### **3-D View of the PCB (Front and Back)**

<img width="1000" height="700" alt="3D Render of the Assembled PCB and Components" src="https://github.com/Zenxta/Security-System-Altium/blob/main/3-D%20(2).png?raw=true" />

<img width="1000" height="700" alt="3D Render of the Assembled PCB and Components" src="https://github.com/Zenxta/Security-System-Altium/blob/main/3-D(1).png?raw=true" />

---

### **Hardware Implementation**

The circuit was verified on a breadboard and permanently assembled on a perforated board and then housed in a custom 3D-printed enclosure.

#### **Final Assembly & Enclosure**

<img width="800" height="600" alt="Testing the soldered PCB with the indicator LED lit" src="https://github.com/Zenxta/Security-System-Altium/blob/main/hdw-1.jpg?raw=true" />

<img width="800" height="600" alt="Final 3D printed enclosure showing the assembled circuit inside" src="https://github.com/Zenxta/Security-System-Altium/blob/main/hwd-3.png?raw=true" />

<img width="800" height="600" alt="Final enclosed product" src="https://github.com/Zenxta/Security-System-Altium/blob/main/hdw-2.png?raw=true" />

