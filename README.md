# PUTM_EV_BMS_HV_SLAVE_2024
Accumulator Managment System (High Voltage Battery Managment System)

## Overview
The AMS system consists of two main parts, the master and multiple slaves.
<p align="center">
  <img src="https://github.com/user-attachments/assets/7aed0fef-9787-402d-a1e4-eb45de333efc">
</p>
The apparatus is responsible for the managment of the battery as a whole, determining it's states like: state of charge or unsafe state plausibility. It also supervises the turning on and off of the hv bus.

## Slave
The AMS Slave is a subsidiary system responsible for measuring all the cell voltages and strategically placed temperatures on one stack.
<p align="center"> 
  <img src="https://github.com/user-attachments/assets/0df92ec7-324f-46ee-9dd0-c78b7227534e">
</p>

### Hardware 
The AMS Slave is powered by LTC6811, a powerful, new gen IC capable of measuring of up to 12 cell simultaneously and up to 5 auxilary readings. One slave features 2 of such IC for a total of 20 cell and 10 temperature measurements. All Slaves are connected in chain configuration allowing for a quick data dump from all slaves in series. For interfacing the LTC6811 uses isoSPI, a special SPI/Ethernet like protocol, which features amazing noise immunity due to usage of a twisted differential pair. All of that on a custom 4 layer board. The AMS slave boasts a lot smaller (106mm x 50mm) size compared to it's predecessor allowing for a lot more versatile usage and making one cell stack far more compact. 

<p align="center"> 
  <img src="https://github.com/user-attachments/assets/36fcfc62-b281-4180-b4c2-4dea0c213393">
</p>

### The research and development work was carried out was a part of the Student Scientific Clubs Create Innovations (SKNTI) program. [Ministry of Science and Higher Education](https://www.gov.pl/web/nauka)
![baner-sknti](https://github.com/PUT-Motorsport/PUTM_VP_SIM/assets/64833115/6471b760-8a2b-4a6e-99b0-7c81398ade27)
