# Greenhouse Ventilation Control System

## PCB and Hardware Design

### Project Overview

This project involved the schematic and PCB design of a **greenhouse automation controller** developed for a client through Upwork. The system is designed to monitor environmental conditions inside a greenhouse and automatically control ventilation systems to maintain optimal growing conditions.

The controller is built around the **Particle Boron 404X microcontroller**, which communicates with **RuuviTag BLE wireless temperature and humidity sensors** installed within the greenhouse. These sensors continuously measure environmental parameters and transmit the data to the controller.

Based on real-time environmental data, the system automatically operates ventilation systems to regulate temperature, humidity, and air circulation.

All system data is transmitted to the **Blynk IoT Platform**, allowing users to remotely monitor greenhouse conditions and system status through a cloud-based dashboard.

This project was completed as part of a freelance collaboration with **GenXI Tech Solutions**.

---

### System Functionality

The system manages two ventilation mechanisms inside the greenhouse:

**GAHT Fan (Ground-to-Air Heat Transfer)**
This fan circulates air through an underground loop to regulate temperature, control humidity levels, and reduce thermal stratification inside the greenhouse.

**HAF Fan (Horizontal Air Flow)**
This fan maintains continuous horizontal air circulation throughout the greenhouse to improve airflow and help reduce plant disease risk caused by stagnant air.

The controller continuously processes environmental sensor data and automatically activates these systems when required.

---

### Hardware Architecture

The hardware system includes the following main components:

Particle Boron 404X microcontroller for system control and cloud connectivity

RuuviTag BLE temperature and humidity sensors for environmental monitoring

ACS712 current sensor for monitoring fan current and detecting possible faults

Relay or switching circuitry for controlling ventilation fans

Power supply and protection circuitry for safe operation

Communication interface with the Blynk IoT cloud platform

---

### PCB Design Details

The hardware was designed as a **two-layer printed circuit board** following standard PCB layout practices for reliability and manufacturability.

Key design features include:

• Separation of high-voltage and low-voltage sections
• 3.2 mm electrical clearance between power domains for safety
• Optimized signal trace widths between 0.25 mm and 0.30 mm
• Wider traces used for power distribution paths
• Solid ground plane to improve signal stability
• Ground stitching vias to enhance noise immunity and reduce EMI
• Careful component placement to fit the project enclosure while maintaining safe electrical spacing

---

### Fault Monitoring

An **ACS712 current sensing module** was integrated into the design to monitor the current drawn by the ventilation fans.

This allows the system to detect abnormal current behavior that may indicate:

• Fan malfunction
• Electrical faults
• Overload conditions

Fault information can be reported through the cloud dashboard.

---

### Manufacturing Outputs

Complete manufacturing outputs were generated to prepare the board for fabrication, including:

• Gerber files
• Drill files
• Bill of Materials (BOM)

The design successfully passed **Design Rule Check (DRC)** with:

0 Errors
0 Warnings
0 Unconnected Nets

This confirms that the PCB is fully ready for manufacturing.

---

### Purpose of the Design

The project demonstrates a practical application of embedded systems and IoT technologies in agriculture. By combining environmental sensing, automated ventilation control, and cloud monitoring, the system provides an efficient solution for greenhouse climate management.

---

### Conclusion

This project highlights the integration of embedded hardware, PCB design, and IoT connectivity to create a reliable greenhouse automation solution. It also demonstrates the application of professional PCB layout practices to ensure electrical safety, signal integrity, and manufacturing readiness.

The design provides a scalable platform for future greenhouse automation systems and further expansion of smart agriculture technologies.
