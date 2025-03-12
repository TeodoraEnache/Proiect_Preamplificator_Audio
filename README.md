# Proiect_Preamplificator_Audio

# 🔊Audio Preamplifier – Design and Implementation
## 📜 Table of contents: 
 -[🔍📖Description](https://github.com/TeodoraEnache/Proiect_Preamplificator_Audio?tab=readme-ov-file#description)
 -[Download Project](https://github.com/TeodoraEnache/Proiect_Preamplificator_Audio?tab=readme-ov-file#download-project)
 -[Project Overview](https://github.com/TeodoraEnache/Proiect_Preamplificator_Audio?tab=readme-ov-file#project-overview)
 -[🔍Circuit Simulation and Testing](https://github.com/TeodoraEnache/Proiect_Preamplificator_Audio?tab=readme-ov-file#circuit-simulation-and-testing)
 -[Conclusion - ⚡Skills Developed](https://github.com/TeodoraEnache/Proiect_Preamplificator_Audio?tab=readme-ov-file#skills-developed)
## 🔍📖Description: 

 A comprehensive project focused on designing and implementing an audio preamplifier with voltage-controlled gain, adjustable between 1x and 40x. The project includes:  
 • Designing the electrical schematic and simulating functionality using Cadence/Orcad PSpice.  
 • Creating a production-optimized SMD-based PCB layout.  
 • Providing detailed documentation, including theoretical analysis, applications, and manufacturing guidelines.

## Download Project:
[👉 📥Click here to download the PDF](https://github.com/TeodoraEnache/Proiect_Preamplificator_Audio/blob/main/Enache_Teodora_Preamplificator%20Audio.pdf)

## Project Overview

 The preamplifier is a crucial component of audio signal processing, enhancing low-level signals from sources such as microphones or pickups to levels that are suitable for further processing or amplification.The design's key feature is its voltage-controlled gain, which allows for precise adjustments to the amplification factor.  
 Adaptability is essential for ensuring audio fidelity in different input signal levels.

 
 ## 🔍Circuit Simulation and Testing

 ### Schematic
 
 The circuit schematic consists of a Darlington amplifier stage, which provides high current gain and high input impedance, making it suitable for low-power signal amplification. The circuit operates with a single positive power supply, using a common ground reference. After amplification and filtering, the processed audio signal is directed to the output stage, ensuring high-quality signal transmission.
 <br/>
![Circuit](https://github.com/TeodoraEnache/Proiect_Preamplificator_Audio/blob/main/schema_electrica.jpg)
 <br/>  

 ### SPICE simulation 

 The result of the SPICE simulation demonstrate how the gain varies with the control voltage.

 #### First Simulation - Control voltage=4V
 The gain is low, when the control voltage is 4V. The output signal(GREEN) is weak, having almost the same amplitude as the imput signal (RED), indicating that the circuit functions as a signal repeater.
 <br/>
![Sim1](https://github.com/TeodoraEnache/Proiect_Preamplificator_Audio/blob/main/VDC%3D4V.jpg)
<br/>

#### Second Simulation - Control voltage=0V
The gain increases, when the control voltage is 0V. The output(GREEN) is amplified significantly, with the output amplitude increased by a factor of 40.
<br/>
![Sim2](https://github.com/TeodoraEnache/Proiect_Preamplificator_Audio/blob/main/VDC%3D0V.jpg)
<br/>

 ### PCB DESIGN
 A custom PCB was designed for the practical implementation of this circuit. The layout optimizes component placement and signal routing to reduce noise and interference, ensuring a clean, amplified output. Measuring 40mm × 40mm, the compact PCB includes dedicated pads for input, output, power connections, and the control voltage signal, making it easily integrable into various audio applications.
 <br/>
![PCB](https://github.com/TeodoraEnache/Proiect_Preamplificator_Audio/blob/main/layout.jpg)
<br/>

## Conclusion - ⚡Skills Developed

Electronic design and simulation.  
• PCB design and layout in SMT technology.  
• Technical documentation and analysis.  
• Proficiency in CAD tools for electronic engineering
