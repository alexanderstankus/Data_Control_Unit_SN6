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


**Layout**
-


**3D View**
- 


