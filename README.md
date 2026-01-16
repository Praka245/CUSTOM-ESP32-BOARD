# ESP32 Custom PCB Design

## 📌 Project Overview

This repository contains the complete design files for a **custom ESP32-based PCB**.  
The project focuses on schematic design, component selection, PCB layout, and manufacturing outputs such as Gerber and NC Drill files.

The design follows standard PCB design practices and is intended for **learning, prototyping, and academic purposes**.

---

## 🛠 Tools Used
<img src="https://github.com/user-attachments/assets/89b5582c-98f2-47cf-a791-ed4f722cd821" width="35" alt="Altium">   <img width="35" height="37" alt="image" src="https://github.com/user-attachments/assets/43e6d5bf-be7a-4a76-913b-2a6f7ce361aa" />

- **PCB Design Software:** Altium Designer
- **Gerber Viewer:** View Mate

---

## 🛠 Key Component and Files

- **Controller:** ESP32  
- **Output Files:** Gerber, NC Drill, BOM  
- **3D Models:** STEP (.stp)

---

## 🔍 Websites used to search Components

The following online resources were used to **search, verify, and download PCB components, footprints, symbols, and 3D models**:

1. **Digi-Key**  
2. **LCSC**
3. **Molex**  
4. **SnapEDA / SnapEDA Magic**
5. **Ultra Librarian** 
6. **3D ContentCentral**

**Note:** For 3D visualization and mechanical verification, **STEP (.stp) files** were downloaded and used.

---

## 📂 Manufacturing Output Files

This repository includes the following fabrication-ready files:

- **Gerber Files** - Copper layers, solder mask, silkscreen  
- **NC Drill Files (.DRR)** - Drill data for vias and holes  
- **Drill Reports (.TXT)** - Hole size and count information  

---

## 👁 Viewing Gerber & NC Drill Files (Optional)

To view and verify Gerber files before fabrication, the following tool was used:

### ViewMate Gerber Viewer

- Open and inspect Gerber layers  
- Verify drill alignment and hole sizes  
- Check PCB before sending to fabrication  

**LINK:** https://www.pentalogix.com/t/software-products/viewmate

---

## 🎯 Project Objectives

- Learn complete PCB design flow  
- Understand component selection and footprint verification  
- Generate fabrication-ready files  
- Practice industry-standard PCB documentation  

---

## 📐 Controlled Impedance Routing (50 Ω)

In this PCB design, **50 Ω characteristic impedance** was maintained for moderate-speed digital signal routing.

### Design Choice

- **Trace Width:** 6 mils  
- **Target Impedance:** 50 Ω  
- **Signal Type:** moderate-speed digital signals  
- **Routing Style:** Single-ended microstrip

The 6 mil trace width was selected based on the **PCB stack-up parameters**, including:
- Dielectric material (FR-4)
- Dielectric thickness between signal layer and reference plane
- Copper thickness
- Presence of a continuous ground reference plane

Using these parameters, impedance calculations confirmed that a **6 mil wide trace achieves approximately 50 Ω** characteristic impedance under the given stack-up conditions.

---

### Why 50 Ω?

- Industry-standard impedance for:
  - High-speed digital signals
  - RF and clock lines
- Minimizes:
  - Signal reflections
  - Impedance mismatch
  - EMI and signal distortion
- Ensures:
  - Signal integrity
  - Reliable data transmission


### Note

- I have calculated the Impedance using the JLPCB's Impedance Calculator based on my **Layer Stackup**

---

## 🔀 Differential Pair Routing

Differential pairs were used in this PCB design for selected high-speed signals to improve signal integrity and noise immunity.

### Why Differential Pairs?

- Transmit signals as a **pair of equal and opposite signals**
- Reduce susceptibility to:
  - External noise
  - EMI (Electromagnetic Interference)
- Improve:
  - Signal integrity
  - Timing accuracy
  - High-speed data reliability

---

<img width="987" height="528" alt="image" src="https://github.com/user-attachments/assets/b4a933a0-17fd-4022-907e-37907ab0ec6c" />

---

### Design Considerations

- **Matched trace lengths** were maintained to minimize skew
- **Consistent spacing** between the differential traces was used to achieve the required **differential impedance**
- Routed over a **continuous reference plane** to ensure stable return paths

---

### Benefits

- Lower common-mode noise
- Reduced radiation and crosstalk
- Suitable for high-speed interfaces such as USB, UART (high-speed), and clock signals


Differential routing ensures robust and reliable communication in high-speed PCB designs.


---

## 📚 Custom Schematic Symbols & Footprints

For some components, **custom schematic symbols and PCB footprints** were created by carefully **referencing the manufacturer datasheets** 📄.

### 🔍 Why Custom Libraries Were Created

- Mainly for designer's convenience 😁

🛠 This approach:
- Simplifies schematic readability 🧩
- Makes routing and placement easier ✨
- Ensures correct pin mapping and package dimensions
- Reduces design errors during layout and fabrication
- Datasheets were used to verify:
  - Pin configuration
  - Pad size and spacing
  - Mechanical outline
- Both **schematic symbols** and **PCB footprints** were validated before layout


Creating custom libraries ensures **correct component placement**, **error-free assembly**, and a **professional PCB design workflow** ✅


---


## 🏭 PCB Manufacturing Considerations (JLCPCB)

The PCB design was created by **referring to JLCPCB’s manufacturing capabilities and design guidelines** to ensure smooth and error-free fabrication 🛠️.

**LINK:** https://jlcpcb.com/capabilities/pcb-capabilities

This includes:
- Trace width and spacing within JLCPCB limits
- Standard drill sizes and via dimensions
- Supported board thickness and copper weight
- Solder mask and silkscreen constraints

---

### ✅ Benefits

- High manufacturability 📈
- Reduced fabrication issues
- Faster turnaround time
- Cost-effective PCB production


Designing within JLCPCB’s capabilities ensures the PCB can be **manufactured reliably without additional modifications** 🔧

---


## SUMMARY:

This project features a custom ESP32-based PCB designed for learning and prototyping. It includes complete schematic capture, component selection, PCB layout, and fabrication-ready files (Gerber, NC Drill, BOM, and STEP). The design ensures signal integrity with controlled impedance routing, differential pair traces for high-speed signals, and is fully manufacturable according to JLCPCB guidelines.

---

### 🙋‍♂️ CONTRIBUTOR

**Prakadeesh N**  
Electronics and Communication Engineering (ECE)  
Interested in VLSI and PSB Design
