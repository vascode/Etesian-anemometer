# Etesian-anemometer
Use Laird RM191 to get wind speed from Etesian anemometer and send that data over LoRa network

### Preparation
LoRa Gateway should be configured so that RM1xx can connect to it and transmit data to it. 
I used [G1xx](https://www.lairdtech.com/products/rg1xx-lora-gateway) gateawy for my testing but any LoRa gateway can be used. 

### Procedure 
1. Start spinning fans of [Etesian anemometer](http://www.etesian-tech.com/dropdown-under-develop/index.html)
2. Run scan.RM1xx.central.sb in RM1xx (RM191 or RM186)

### What you will see
BLE peripheral of Etesian anemometer will advertise with following information
- Device ID
- Temperature
- Wind speed
- Wind direction

RM1xx will recieve these data in BLE and send them over to LoRa gateway through LoRa network. 
