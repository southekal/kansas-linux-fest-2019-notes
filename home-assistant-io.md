### title: linux based home automation with home-assistant.io
### speaker: [kyle sheumaker](https://kansaslinuxfest.org/kyle-sheumaker/)
### date: 08112019

#### notes:
- connecting all individual iot devices together
- motion sensors
- many different protocoals for connecting devices
  - z-wave
  - zigbee(shorter distance than z-wave eg: hue, ikea, doesnt require standardization) 
  - wifi(high power consumption, constantly connected as compared to z-wave/zigbee)
  - lutron, insteon, 433mhz devices
  - others
- home automation hub connects all these things together.
- commercial options include: samsung, apple
- cloud based home automation has outage issues, security and privacy issues, lack of control
- home assistant:
  - py implementation
  - 1450 integrations
  - simple to extend
  - common deployment is raspberry pi3
- getting started:
  - `hass.io` for raspberry
  - access hassio.local:port
  - `configuration.yaml` (has `secrets.yaml` for api keys/secrets)
  - do things like speedtest for eg: ping/download/upload
- node-red: integrates with home-assistant if you dont wanna use `yaml`
- buy your own sensors: sonoff switch (amazon/aliexpress); firmware is questionable
- esp8266 microcontroller: lok for them
- tasmota (firmware replacement)
- esp home (firmware replacement)
- garage door sensor: wemos d1 mini microcontroller; ultrasonic distance sensor
- gateways and hubs:
  - aeotech z-stick
  - deconz conbee2
  - lutron caseta
- lighting:
  - ikea (zigbee)
  - caseta wall dimmer (lutron hub)
  - magic home led strip (wifi)
  - kuled switch (wifi)
- climate:
  - ecobee thermostat (open api)
  - ge ceiling fan controller (z-wave)
  - keen smart vents (zigbee)
  - lutron serena shades (lutron hub)
- misc devices:
  - schlage door lock (has key backup/ z-wave)
  - amazon echo
  - dome water leak sensor (zwave)
  - rca doorbell
- when possible stay away from cloud devices
- replace light switch with smart switch
- network security: z-wave and zigbee

