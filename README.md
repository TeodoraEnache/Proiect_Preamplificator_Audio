
# 🔊Audio Preamplifier with Voltage-Controlled Gain – Design and Implementation

## Academic Context
### National University of Science and Technology POLITEHNICA Bucharest  
#### Faculty of Electronics, Telecommunications, and Information Technology  
##### Academic Year 2024-2025 
**Supervisors:**  
- Prof. Dr. Eng. Dragoș Dobrescu  
- Lecturer Dr. Eng. Mădălin Moise  

##  Table of Contents  

1. [ Description](#-description)  
2. [ Download Project](#download-project)  
3. [ Project Overview](#project-overview)  
4. [ Circuit Simulation and Testing](#-circuit-simulation-and-testing)  
   - [ Schematic](#schematic)  
   - [ SPICE Simulation](#spice-simulation)  
     - [First Simulation - Control voltage = 4V](#first-simulation---control-voltage4v)  
     - [Second Simulation - Control voltage = 0V](#second-simulation---control-voltage0v)  
5. [PCB Design](#pcb-design)  
   - [ PCB Layout](#pcb-layout)  
6. [Audio Preamplifier - PCB Layers](#audio-preamplifier---pcb-layers)  
   - [🔷 TOP Layer](#-top-layer)  
   - [🔷 BOTTOM Layer](#-bottom-layer)  
   - [🔷 SMTOP Layer (Solder Mask Top)](#-smtop-layer-solder-mask-top)  
   - [🔷 SMBOT Layer (Solder Mask Bottom)](#-smbot-layer-solder-mask-bottom)  
   - [🔷 SSTOP Layer (Silkscreen Top)](#-sstop-layer-silkscreen-top)  
   - [🔷 Outline Layer (Board Outline)](#-outline-layer-board-outline)  
   - [🔷 Fabrication Layer](#-fabrication-layer) 
7. [Repository Contents](#repository-contents)
8. [Conclusion](#conclusion)
9. [References](#references)


## Project Description: 

 A comprehensive project focused on designing and implementing an audio preamplifier with voltage-controlled gain, adjustable between 1x and 40x. The project includes:  
 • Designing the electrical schematic and simulating functionality using Cadence/Orcad PSpice.  
 • Creating a production-optimized SMD-based PCB layout.  
 • Providing detailed documentation, including theoretical analysis, applications, and manufacturing guidelines.

## Download Project:
[Click here to download the Project as PDF](https://github.com/TeodoraEnache/Proiect_Preamplificator_Audio/blob/main/Enache_Teodora_Preamplificator%20Audio.pdf)

## Project Overview

 The preamplifier is a crucial component of audio signal processing, enhancing low-level signals from sources such as microphones or pickups to levels that are suitable for further processing or amplification.The design's key feature is its voltage-controlled gain, which allows for precise adjustments to the amplification factor.  
 Adaptability is essential for ensuring audio fidelity in different input signal levels.

 
 ## Circuit Simulation and Testing

 ### Schematic
 
 The circuit schematic consists of a Darlington amplifier stage, which provides high current gain and high input impedance, making it suitable for low-power signal amplification. The circuit operates with a single positive power supply, using a common ground reference. After amplification and filtering, the processed audio signal is directed to the output stage, ensuring high-quality signal transmission.
 <br/>
![Circuit](https://github.com/TeodoraEnache/Proiect_Preamplificator_Audio/blob/main/Images/schema_electrica.jpg)
 <br/>  

 ### SPICE simulation 

 The result of the SPICE simulation demonstrate how the gain varies with the control voltage.

 #### First Simulation - Control voltage=4V
 The gain is low, when the control voltage is 4V. The output signal(GREEN) is weak, having almost the same amplitude as the imput signal (RED), indicating that the circuit functions as a signal repeater.
 <br/>
![Sim1](https://github.com/TeodoraEnache/Proiect_Preamplificator_Audio/blob/main/Images/schema_electrica.jpg)
<br/>

#### Second Simulation - Control voltage=0V
The gain increases, when the control voltage is 0V. The output signal(GREEN) is amplified significantly, with the output amplitude increased by a factor of 40.
<br/>
![Sim2](https://github.com/TeodoraEnache/Proiect_Preamplificator_Audio/blob/main/Images/VDC%3D0V.jpg)
<br/>

 ### PCB DESIGN
 A custom PCB was designed for the practical implementation of this circuit. The layout optimizes component placement and signal routing to reduce noise and interference, ensuring a clean, amplified output. Measuring 40mm × 40mm, the compact PCB includes dedicated pads for input, output, power connections, and the control voltage signal, making it easily integrable into various audio applications.

 #### **Layout**

![PCB](https://github.com/TeodoraEnache/Proiect_Preamplificator_Audio/blob/main/Images/layout.jpg)


### Audio Preamplifier - PCB Layers
#### 🔷 **TOP Layer** 
![TOP](https://github.com/TeodoraEnache/Proiect_Preamplificator_Audio/blob/main/Images/TOP.png)
- Contains **all electronic components**, as per project requirements.
- Signal, power, and interconnection traces.
- Fiducial markers for precise alignment in the SMT assembly process.
#### 🔷 **BOTTOM Layer**
![BOTTOM](https://github.com/TeodoraEnache/Proiect_Preamplificator_Audio/blob/main/Images/BOTTOM.png)
- Used for additional traces and interconnection through **vias (0.4mm diameter)**.
- Helps optimize circuit routing.
#### 🔷 **SMTOP Layer** *(Solder Mask Top)*
![SMTOP](https://github.com/TeodoraEnache/Proiect_Preamplificator_Audio/blob/main/Images/SMTOP.png)
- A protective layer that covers exposed copper traces, preventing oxidation and short circuits.
- Only exposes the necessary soldering pads.

#### 🔷 **SMBOT Layer** *(Solder Mask Bottom)*
![SMBOT](https://github.com/TeodoraEnache/Proiect_Preamplificator_Audio/blob/main/Images/SMBOT.png)
- Similar to SMTOP but applied to the bottom side of the board.
- Protects traces on the BOTTOM layer.

#### 🔷 **SSTOP Layer** *(Silkscreen Top)*
![SSTOP](https://github.com/TeodoraEnache/Proiect_Preamplificator_Audio/blob/main/Images/SSTOP.png)
- A labeling layer containing component markings and assembly references.
- Must not overlap soldering pads.

#### 🔷 **Outline Layer** *(Board Outline)*
![Outline](https://github.com/TeodoraEnache/Proiect_Preamplificator_Audio/blob/main/Images/Outline.png)
- Defines the PCB dimensions (**40mm x 40mm**).
- Includes the **(0,0) coordinate** origin mark in the bottom-left corner.
#### 🔷 **Fabrication Layer**
![Fabrication](https://github.com/TeodoraEnache/Proiect_Preamplificator_Audio/blob/main/Images/Fabrication.png)
- Contains essential manufacturing information.

### Repository Contents
The repository includes essential design files:

Schematics: Detailed circuit diagrams illustrating the preamplifier's design.

Layout: PCB layout designs for the physical implementation of the circuit.

Gerber and Excellon Files: Manufacturing files necessary for PCB fabrication.

The project and its official documentation are available as a PDF.
 
 ### Conclusion 
 *This audio preamplifier project not only demonstrates the integration of theoretical and practical knowledge in audio electronics but also highlights the importance of a well-optimized PCB design. The carefully structured PCB layout ensures minimal noise, efficient signal routing, and proper thermal management, crucial for maintaining high-fidelity audio performance. By implementing a voltage-controlled gain feature and utilizing a compact, production-ready SMD layout, this design provides a scalable and reliable solution for various audio amplification needs.*

 ### References 
 1. Brezeanu,Gheorghe. Draghici, Florin. **Circuite Electronice fundamentale**, Ed. Niculescu (2013)
 2. Codreanu, Norocel. **Platforme Laborator Tehnici CAD de Realizare a Modulelor Electronice** (n.d.)
 3. Mitzner, K. **Complete PCB design using OrCAD Capture and PCB editor**, Newnes, 2009
 4. Popa, Cosmin Radu. **Platforma laborator** CIA (n.d.)