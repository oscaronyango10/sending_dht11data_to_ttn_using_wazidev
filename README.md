# Sending-parameters-from-sensors-to-TTN-using-wazidev
I have been trying to send data from sensors using wazidev board. The node only sends data once.
I researched on the connection of RFM95/96  and the microcontroller and the connections are found here. 

// C. Pham's ProMini PCB (wazidev v1.3) 
// Pin mapping
 
const lmic_pinmap lmic_pins = {
  .nss = 10,
  .rxtx = LMIC_UNUSED_PIN,
  .rst = 4,
  .dio = {2, 3, LMIC_UNUSED_PIN},
};
the code is now working well. 

Data to ttn images

![image](https://user-images.githubusercontent.com/52659391/110303669-b3889380-800b-11eb-95ee-dc608041e29f.png)


<<========= sending data to Firebase from the things cloud to firebase ======================>>

Go to Integrations -> add integration

choose HTTP integration
in the process id enter your topic of choice

access key choose ----> default key 

URL ----> Enter the link form firebase and add /data.json at the end of the link eg https://iotlab2021dev1-default-rtdb.firebaseio.com/data.json

Methond -----> POST

Leave other blank then save

see image below 
![image](https://user-images.githubusercontent.com/52659391/110303523-8805a900-800b-11eb-981a-7d8eaa65cc19.png)


data getting in database
![image](https://user-images.githubusercontent.com/52659391/110300926-92727380-8008-11eb-9798-4d28842385c9.png)


images of data in firebase 

![image](https://user-images.githubusercontent.com/52659391/110300780-5b9c5d80-8008-11eb-8ea1-4e923fca2141.png)
 



