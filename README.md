# Stairsgit
Sample RFID Employee login project based on Qt/C++11 &amp; LoRaWAN™ which is a Low Power Wide Area Network (LPWAN). Hardware used is Waspmote by Libellium.

LoRaWAN is a new, private and spread-spectrum modulation technique which allows sending data at extremely low data-rates to extremely long ranges. The low data-rate (down to few bytes per second) and LoRaWAN modulation lead to very low receiver sensitivity (down to -136 dBm), which combined to an output power of +14 dBm means extremely large link budgets: up to 150 dB, what means more than 22km (13.6 miles) in LOS links and up to 2km (1.2miles) in NLOS links in urban environment (going through buildings).
Libelium's LoRaWAN 868 module works in both 868 and 433MHz ISM bands (and the LoRaWAN 900 module works in 900MHz ISM band), which makes it suitable for virtually any country. Those frequency bands are lower than the popular 2.4 GHz band, so path loss attenuation is better in LoRaWAN. In addition, 868 and 900MHz are bands with much fewer interference than the highly populated 2.4 GHz band. Besides, these low frequencies provide great penetration in possible materials (brick walls, trees, concrete), so these bands get less loss in the presence of obstacles than higher band.
With the LoRaWAN modules we can send the data directly to any Base Station (BS) that is LoRaWAN compatible. Some companies already offering solutions are: Kerlink, Link-Labs, Multitech, Cisco, Augtek, Manthink, Gupsy, Gemteck, ExpEmb, Embedded Planet, Calao, RFI, etc. In order to visualize the information we will need also a Cloud platform where the data has to be sent. Normally when you acquire a BS you can install your preferred SW packet in order to make it work against the Cloud platform. We tested the RFID LoRaWAN radio solution with Kerlink gateway connected to "thethingsnetwork" Cloud platform (www.thethingsnetwork.com) which is based on REST & MQTT, the MQTT version is not included here in this project. 

The waspmote modules may be used in two different more configurations.

P2P Mode - Direct Communication between nodes (LAN Interface)
Hybrid Mode - LoRaWAN / P2P (P2P + GW to LoRaWAN Network)
In the P2P Mode nodes may connect directly among them and send messages directly at no cost (as they are not using the LoRaWAN Network but just direct radio communication). This is useful as we can create secondary networks at any time as we don't need to change the firmware but just use specific AT Commands in the current library. This mode works without the need of a Base Station or a Cloud account so in case you don't want to purchase any license (or renew the license after the initial period) you will be able to keep on using the modules this way. For more info go to the section P2P Mode.

Note: the links in the project will not work as they are connected to the units we have used.

Fore more information on the waspmote & tutorial, refer the website:  https://www.cooking-hacks.com/documentation/tutorials/lorawan-for-arduino-raspberry-pi-waspmote-868-900-915-433-mhz 
