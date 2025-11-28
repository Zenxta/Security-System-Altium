This project develops a low-cost and reliable Security Alarm System utilizing a Bipolar Junction Transistor (BJT) and a Silicon-Controlled Rectifier (SCR).
The system's core mechanism detects unauthorized access by sensing interruptions in an Infrared (IR) beam. The critical feature is the use of the SCR, which ensures a latching mechanism—the alarm remains active until manually reset, even if the triggering event is brief.

### **Key Features**

* **Sensing Mechanism:** Uses an invisible **IR LED** and **IR Photodiode** setup, providing an advantage over visible light systems.
* **Persistent Alert:** A **TYN612 SCR** provides the critical latching function. Once triggered, the alarm remains ON until manually reset, ensuring brief intrusions are not missed.
* **Adjustable Sensitivity:** A **$100\ k\Omega$ Potentiometer** allows the user to fine-tune the circuit's sensitivity for different environmental conditions.
* **Power & Enclosure:** Powered by rechargeable **18650 Li-ion cells** with a **TP4056 charging module** (Type-C) and protected by a custom 3D-printed enclosure.

### **Components**

| Component | Type | Quantity | Key Role |
| **Transistor** | BC547 (BJT) | 1 | Amplifies the weak photodiode signal to trigger SCR|
| **Latching Device** | TYN612 (SCR) | 1 | Maintains alarm status until power is interrupted|
| **Sensing Pair** | IR LED, IR Diode | 1, 1 | Creates and detects the invisible security beam|
| **Adjuster** | Potentiometer ($100\ k\Omega$) | 1 | Fine-tunes the tripping point/sensitivity|
| **Output** | Buzzer | 1 | Audible alert signal|

### **Design Files & Visualization**

The Schematic and PCB Layout were designed using Altium Designer software.

#### **Schematic Diagram**

<img width="1200" height="800" alt="Schematic Diagram of the BJT-SCR Security Alarm Circuit" src="" />

#### **PCB Layout**

<img width="1200" height="800" alt="PCB Layout for the BJT-SCR Security Alarm" src="" />

#### **3-D View of the PCB (Front and Back)**

<img width="1000" height="700" alt="3D Render of the Assembled PCB and Components" src="" />

---

### **🔨 Hardware Implementation**

The circuit was verified on a breadboard and permanently assembled on a perforated board, then housed in a custom 3D-printed enclosure.

#### **Breadboard Prototype**

Initial testing was conducted on a breadboard to verify circuit flow and functionality.

<img width="800" height="600" alt="Breadboard connection of the Alarm Security System" src="[INSERT FIGURE 5.1 BREADBOARD IMAGE URL HERE]" />

#### **Final Assembly & Enclosure**

The final circuit was soldered for stability and integrated into an enclosure designed in Autodesk Fusion to house the electronics, battery, and charging port.

<img width="800" height="600" alt="Testing the soldered PCB with the indicator LED lit" src="" />

<img width="800" height="600" alt="Final 3D printed enclosure showing the assembled circuit inside" src="" />

### **Project Files**

All files required for manufacturing and design review are included in the repository.

* **Schematic:** `Security_Alarm_System.SchDoc`
* **PCB Layout:** `Security_Alarm_System.PcbDoc`
* **Gerber Files:** `Gerber_Files.zip`


### **Future Work**

The system can be enhanced with modern technology to improve functionality:

* **Microcontroller Integration:** Incorporating an Arduino or ESP32 to enable advanced features like automatic alarm reset, timed alerts, and data logging
* **Wireless Notifications:** Integrating a GSM module or IoT system to send SMS alerts or app notifications upon intrusion
