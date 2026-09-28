
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
<img width="1018" height="803" alt="DCU_sch_s4" src="https://github.com/user-attachments/assets/9a9d182b-90cb-4925-a1c0-43512db4060a" />
<img width="1018" height="803" alt="DCU_sch_s3" src="https://github.com/user-attachments/assets/1327c1f1-eab0-48e2-9233-4bfc953eaa31" />
<img width="1017" height="805" alt="DCU_sch_s2" src="https://github.com/user-attachments/assets/c1e0b860-e0af-44b8-bd0f-4ee1303c287c" />
<img width="722" height="685" alt="DCU_Layout" src="https://github.com/user-attachments/assets/e8738c5c-390a-43cb-b7a9-7f8b901932bc" />


**Layout**
-


**3D View**
- 


