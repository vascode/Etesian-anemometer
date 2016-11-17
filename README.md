# Etesian-anemometer
Use Laird RM191 to get wind speed from Etesian anemometer and send that data over LoRa network

###Preparation
LoRa Gateway should be configured so that RM1xx can connect to it and transmit data to it. 
I used Mutitech gateawy for my testing but any LoRa gateway can be used. 

###Procedure 
1. Start [Etesian anemometer](http://www.etesian-tech.com/dropdown-under-develop/index.html)
2. Run scan.BL620.sb in RM1xx (RM191 or RM186)

###What you will see
BLE peripheral in Etesian anemometer will advertise with following information
- Temperature
- Wind speed
- Wind direction

RM1xx will recieve these data and send them over to LoRa gateway. 
