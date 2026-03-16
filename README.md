# Home Assistant Setup – Smart Home Overview

This document describes the structure and design of my Home Assistant environment.  
The goal of this setup is to create a **stable, scalable, and maintainable smart home system** using reusable automations, sensors, and blueprints.

The system is designed with the following principles:

- **Automation first**
- **Reusable configuration**
- **Minimal duplication**
- **Hardware-agnostic design**
- **Stable long-term operation**

---

# System Overview

The Home Assistant environment is used to control and automate several aspects of the house, including:

- Lighting automation
- Motion detection
- Environmental monitoring
- Energy and power monitoring
- Appliance notifications
- Sensor integrations
- Zigbee device control
- Smart automation based on **lux, motion, and presence**

The setup is primarily built around **Zigbee sensors, smart switches, and environmental sensors**, with additional integrations for WiFi and network-based devices.

---

# Hardware

## Host System

- **Raspberry Pi 4**
- **4 GB RAM**
- Running **Home Assistant OS**

---

## Zigbee Devices

Zigbee devices are connected through a dedicated coordinator and managed through Home Assistant.

**Coordinator**

- SONOFF ZigBee 3.0 USB Dongle Plus

**Sensors and Devices**

- Tuya Zigbee 4-in-1 Radar Motion Sensor  
  (Motion, illuminance, temperature, humidity)
- IKEA Inspelning smart plug  
  *(primarily used for power monitoring)*
- TRÅDFRI LED Bulb E27 250 lumen  
  *(smart wireless dimmable warm white globe)*
- SONOFF ZBMINIL2
- SONOFF ZBMINI
- SONOFF SNZB-04 door/window sensor

---

## WiFi & Network Devices

These devices connect directly to the network and integrate with Home Assistant through native integrations or APIs.

- TP-Link Tapo P110 smart plugs  
  *(primarily used for power monitoring)*
- TP-Link Tapo C510W camera
- Dreame D10 Plus Gen 2 robot vacuum
- HomeWizard P1 energy meter
- Sony Android TVs

---

## Other Devices

Additional smart home devices integrated into the system:

- Motionblinds gateway
- Motionblinds roller blinds

---

## Future Hardware / Expansion

The system is designed to support future expansion.

Planned additions include:

- Bluetooth tracking
- ESP32-based sensors
- Custom ESPHome devices
- Additional environmental sensors
- Room-level presence detection

Currently, i have several **ESP32 devices** are available but not yet actively used in the setup.

These will be integrated in future iterations of the smart home environment.