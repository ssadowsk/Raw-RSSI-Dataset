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
A set of tests was conducted to determine the accuracy between multiple types of system designs including: Trilateration, Fingerprinting with K-Nearest Neighbor (KNN) postprocessing, while using filtering types such as: Running Average and Kalman. 
 
 ## Environment
The experimental environment utilized was a 5.8 x 5.3 m meeting room. The environment was a very noisy environment due to a large number of transmitter being in the area at the time the experiments were performed. All points were taken when on tables to simulate a constant height between all the points. 
 
 ## Topology
 In the testing environemnt, 16 fingerprints were gathered to be used in the creation of a database, while 6 points were selected to be used against the database for the comparison. A general overview of the experiment performed can be seen in:
 
 Fingerprints             |  Test Points
:-------------------------:|:-------------------------:
![](https://github.com/ssadowsk/Raw-RSSI-Dataset/blob/master/Images/fingerprints.png)  |  ![](https://github.com/ssadowsk/Raw-RSSI-Dataset/blob/master/Images/tests.png)
 
 # Related Publications
 
 To be added...
 
 # Dataset
The RSSI dataset is seperated based on wireless technology (i.e. WiFi, BLE, and Zigbee). Each folder contains three additional folders seperating where the data was gathered (Pathloss, Database, and Tests). Pathloss contains 18 files measuring the RSSI at varying distances from the devices. Database contains 16 files measuring the RSSI at the fingerprint locations from the three transmitters. Tests contains 6 files measuring the RSSI at random locations which will be used for performing testing with. 

For each technology the file name corresponds to the point as to where the data was gathered. For specific locations, the (x,y) coordinates can be seen in the appropiate .xlsx file.

For each file there are approximatly 300 reading in the format "Node *Letter*: *Value*" where:
*Letter* corresponds to the transmitter that signal was sent from, represented by 'A', 'B', or 'C'.
*Value* is the RSSI reading.
