# DomoHome
This is an umbrella project for multiple projects related to domotics using ESP-based devices. 

A DomoHome installation will consist of an offline-first (only local network required) hub that will be controlled by means of a web application accessible in the local network. 
Multiple devices will connect to the hub so that they can be managed through the web application.

## Structure (git submodules)
- `domohome-hub` - ESP8266 C++ using PlatformIO. Entry: `src/main.cpp`
- `domohome-hub-ui-web` - React + TypeScript + Vite (builds assets for hub)
- `domohome-devices` - Peripheral device code

## domohome-hub
- **Build**: `pio run` (PlatformIO)
- **Setup**: Copy `include/credentials.example.h` to `include/credentials.h`, fill WiFi credentials
- **Framework**: Arduino/ESP8266

## domohome-hub-ui-web
- Standard Vite React app
- Build output goes to `dist/`, served by hub's web server

## domohome-devices
this is going to be another PlatformIO project containing a colleciton of ESP-based devices like lightbulbs, cameras, switches, and so on...