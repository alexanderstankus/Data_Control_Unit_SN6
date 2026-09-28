
# Data_Control_Unit_SN6
Data Control Unit PCB for UC Berkeley's Formula Electric SN6 race car in the FSAE Electric competition.
-

**Overview**
- 
The DCU (Data Control Unit) for Formula Electric at Berkeley's SN6 vehicle is designed to transmit data from the car to our pit. With a LoRa radio transceiver, this board sends data to a wireless transceiver that uploads data to a local computer to get real-time updates on performance and any critical information that the team needs to know at any given time. This year's new implementation on the board is Texas Instruments' ST67 IC, which allows us to send data OTA via wifi and Bluetooth. This IC acts as a wifi extension to our STM32 MCU. In addition, this board now features a USBC for flashing data instead of an ST-Link. 

**Features**
- 
* Dual CAN-Bus interface: Supports 2 CAN inputs (CAN1 and CAN2) for robust system communication (Especially important for a board controlling safety systems)
* LoRa Radio Transceiver: Wireless data transmission
* ST67 Wifi Module: Faster OTA data transmission + TCXO clock to prevent frequency breakdown under heat stress
* SD Card for local data upload/downloads
* High-current power switching: Several different types of converters, like LDO and Buck Converters (step-down for components + Power regulation for MCU)
* Ideal diodes for reverse current protection
* USBC for flashing code

**Schematic**
-
<img width="1040" height="771" alt="DCU _sch_s1" src="https://github.com/user-attachments/assets/6eb4e5f5-b735-42f6-a869-9646ff346d4f" />
*Schematic Sheet 1: Contains the CAN Connector (MX150), USBC set in Full Speed Configuration, LoRa Radio Implementation, SD Card Holder, and ST67 Wifi Module with a TCXO.*


<img width="1018" height="803" alt="DCU_sch_s3" src="https://github.com/user-attachments/assets/1327c1f1-eab0-48e2-9233-4bfc953eaa31" />
*Schematic Sheet 2: Contains the Microbasic module with an STM32 MCU and a UPS Block Set Up to prevent voltage drop and corruption on all components using +5V or +3.3V.*


<img width="1017" height="805" alt="DCU_sch_s2" src="https://github.com/user-attachments/assets/c1e0b860-e0af-44b8-bd0f-4ee1303c287c" />
*Schematic Sheet 3: Contains all LDOs and Buck Converters used to step the voltage down from +24V to +5V to +3.3V. Also contains ideal diode ICs for reverse-current protection.*


<img width="1018" height="803" alt="DCU_sch_s4" src="https://github.com/user-attachments/assets/9a9d182b-90cb-4925-a1c0-43512db4060a" />
*Schematic Sheet 4: Contains the TPS block to regulate our +24V raw from the battery pack to +24V to power the board.*


**Layout**
-
<img width="722" height="685" alt="DCU_Layout" src="https://github.com/user-attachments/assets/e8738c5c-390a-43cb-b7a9-7f8b901932bc" />
*Layout: 4 layer board utilizing 4 ground pours.*


**3D View**
- 
<img width="722" height="811" alt="Screenshot 2026-09-27 at 7 07 49 PM" src="https://github.com/user-attachments/assets/d2af4a91-a69b-4a54-9db7-7879e835929e" />


*Additional PDF featuring the Schematic and Layout can be found in the exports folder within the repo*

Designed on Altium Designer by Alexander Stankus

GitHub: @alexanderstankus

Email: alexstankus99@gmail.com

