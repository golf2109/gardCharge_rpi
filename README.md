# gardCharge for rpi

This is a Beta Python software for enabling GardCharge GC101 
Smart USB Timer Charger Protector or GardCharge GC101PM Smart
USB Power Meter hardware device to work as Data-Acquisition
Unit (for reading Voltage, Current, and Power info) wirelessly 
connected via Bluetooth Low Energy (BLE) on a Raspberry Pi.  
Note that this Beta software only works as one-direction data 
reading from GardCharge (Tx) to Raspberry Pi (Rx), while not able 
to send control command from Raspberry Pi (Tx) to GardCharge (Rx).
 
It will be great for those who are more knowledgeable on 
Raspberry Pi’s BLE Tx to further support the cause to make GardCharge 
work BOTH as Data Acquisition (Rx) AND as Command Control (Tx) device.
 
Nonetheless, GardCharge as Data-Acquisition Unit 
(for Voltage / Current / Power data sensing) alone for Raspberry Pi 
may perform for various IoT applications.

# measure data:
    Voltage , Current , Watt , mAH

# install bluepy
    $sudo install bluepy
    
Test on: 
    raspberry pi 3 model B
    raspberry pi 3 model A+
    
# Gardcharge BLE Service & Characteristic:
    tx_service_UUID          = "FFF0"
    tx_Characteristic_UUID   = "FFF5"
    rx_service_UUID          = "FFE0"
    rx_Characteristic_UUID   = "FFE2" (notification)

