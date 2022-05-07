# macropad

## Introduction
A low-budget macro numeric keypad based on ESP32 MCU and CH9329 USB HID emulation chip.

## Functions
### Keys and Layout
1. Standard 10-key layout + 5 function keys
2. All key macro support
3. Up to 5 macro profiles (stored in MCU's internal storage)

### Connectivity
1. USB 2.0 HID (CH9329 based) 
2. Built-in USB hub, 1 external USB port, 1 internal USB (based on FE1.1s)
3. USB UART debugging (based on CH340C)
4. Bluetooth 4.2 BLE HID   
5. 2.4GHz Wi-Fi (for configuration and OTA firmware update)

### Power Supply & Power Management
1. 3.7V Li-ion battery charging and management (based on TP5400)
2. Supports MCU's deep sleep and hibernation. 

### UI & User Interaction
1. 0.91' built-in I2C OLED screen
2. Cross-platform configuration App on PC using Qt/PyQt
3. Web configuration interface

### Others
1. USB HID Mouse emulation
2. TBD
