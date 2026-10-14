# DeskMoodLight
A custom 3D-printed, Wi-Fi-enabled smart desk mood lamp powered by an ESP32 and ESPHome, featuring addressable WS2812B LEDs and smooth geometric diffusion.

## Overview
DeskMoodLight is a local-first smart ambient lamp designed to sit on a desk or workspace. It integrates natively with Home Assistant via ESPHome, allowing for smooth color transitions, dynamic lighting effects (like fire and rainbows), and physical control. 

## Features
- **Addressable RGB:** WS2812B LED strip for smooth color gradients and dynamic effects
- **Local Control:** Powered by ESPHome & Home Assistant (no cloud required)
- **Custom 3D-Printed Diffuser:** Designed in Fusion 360 to eliminate LED hotspots and evenly scatter light
- **Compact & Clean:** Powered via a single USB-C cable with an internal ESP32 microcontroller

## Hardware Bill of Materials (BOM)
- ESP32 Development Board (NodeMCU / DevKit)
- WS2812B Addressable LED Strip (5V, 60 LEDs/m)
- 5V 3A USB-C Power Supply
- Translucent White PETG Filament (for 3D printing the diffuser shell)

## Firmware Setup
Flash the `mood-light.yaml` configuration to your ESP32 using ESPHome CLI or Home Assistant dashboard integration.
