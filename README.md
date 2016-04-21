# Compilation notes
`cmake -DCMAKE_BUILD_TYPE=Release .`
`make`

# About this fork
Domoticz uses a lot of `sleep_seconds(1);` calls, that delays most of the actions that I need to be almost instant (turning lights ON/OFF for instance).

I replaced those calls by `sleep_milliseconds(50);` without knowing if this would negatively impact the app. For now, it's working as intended.

# Domoticz

Domoticz is a Home Automation System that lets you monitor and configure various devices like: Lights, Switches, various sensors/meters like Temperature, Rain, Wind, UV, Electra, Gas, Water and much more. Notifications/Alerts can be sent to any mobile device

## Multi platform: Linux/Windows/Embedded Devices

This system is designed to operate in various operating systems.
The user-interface is a scalable HTML5 web frontend, and is automatically adapted for Desktop and Mobile Devices.
Compatible with all recent browsers

Some Information
- Hardware: RFXCOM Transciever, Z-Wave, P1 Smart Meter, YouLess Meter, Pulse Counters, 1-Wire, Philips Hue and a lot more....
- Extended logging
- iPhone / Android push notifications
- Auto Learning sensors/switches
- Manual creation of switch codes
- Share / Use external devices
- Designed for simplicity

# More information
* Website: http://www.domoticz.com
* Forum http://www.domoticz.com/forum
* Wiki http://www.domoticz.com/wiki

### Build Status

Status | Operating system
------------ | -------------
![image](https://travis-ci.org/domoticz/domoticz.svg?branch=master "Linux Build Status") | Linux x86_64
![image](https://ci.appveyor.com/api/projects/status/fskiwvjs1q7svwq9?svg=true "Windows Build Status") | Windows
