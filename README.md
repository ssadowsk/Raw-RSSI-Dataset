# Raw-RSSI-Dataset

This RSSI Dataset is a comprehensive set of Received Signal Strength Indicator (RSSI) readings gathered from within a meeting room. Three wireless technologies were used consisting of:
 - WiFi (IEEE 802.11n 2.4GHz band)
 - Bluetooth Low Energy (BLE) and
 - Zigbee (IEEE 802.15.4)
 
 For the experimentation, the equipment utilized consisted of Raspberry Pi 3 Model Bs, Gimbal Series 10 Beacons, and Series 2 Xbees with Arduino Uno microcontrollers.
 
  <p align="center">
Equipment used in experimentation
<img src="https://github.com/ssadowsk/Raw-RSSI-Dataset/blob/master/Images/equipment.jpg">
 </p>
 
 # Experiment
 
 ## Environment
 
 ## Topology
 
 Fingerprints             |  Test Points
:-------------------------:|:-------------------------:
![](https://github.com/ssadowsk/Raw-RSSI-Dataset/blob/master/Images/fingerprints.png)  |  ![](https://github.com/ssadowsk/Raw-RSSI-Dataset/blob/master/Images/tests.png)
 
 # Related Publications
 
 To be added...
 
 # Dataset
The RSSI dataset is seperated based on wireless technology (i.e. WiFi, BLE, and Zigbee). Each folder contains three additional folders seperating where the data was gathered (Pathloss, Database, and Tests). Pathloss contains 18 files measuring the RSSI at varying distances from the devices. Database contains 16 files measuring the RSSI at the fingerprint locations from the three transmitters. Tests contains 6 files measuring the RSSI at random locations which will be used for performing testing with. 

For each technology the file name corresponds to the point as to where the data was gathered. For specific locations, the (x,y) coordinates can be seen in the appropiate .xls file.

For each file there are approximatly 300 reading in the format "Node *Letter*: *Value*" where:
*Letter* corresponds to the transmitter that signal was sent from, represented by 'A', 'B', or 'C'.
*Value* is the RSSI reading.
