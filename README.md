# Sending-parameters-from-sensors-to-TTN-using-wazidev
I have been trying to send data from sensors using wazidev board. The node only sends data once.
I researched on the connection of RFM95/96  and the microcontroller and the connections are found here. 

// C. Pham's ProMini PCB
// Pin mapping
 
const lmic_pinmap lmic_pins = {
  .nss = 10,
  .rxtx = LMIC_UNUSED_PIN,
  .rst = 4,
  .dio = {2, 3, LMIC_UNUSED_PIN},
};
the code is now working well


