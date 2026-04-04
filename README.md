# DomoHome

A domotics system for your home.

This project is comprised of multiple git submodules:

## domohome-hub

The central hub where all the devices connect

- Runs an MQTT broker that serves as a means of communication between all the devices, including the hub itself
- Runs a simple web server that serves a UI interface to manage the hub

## domohome-hub-ui-web

A web interface for the hub.

When built, produces the assets served by the hub's web server.

## domohome-devices

A collection of peripheral devices like lightbulbs and thermostats.
