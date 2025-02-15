---
manufacturer: Xiaomi/MiaoMiaoCe
name: "Alarm clock"
model: MHO-C401
image: "MHO-C401.jpg"
physical_description: "Small square body, E-Ink display"
broadcasted_properties:
  - temperature
  - humidity
  - battery
  - voltage
  - rssi
broadcasted_property_notes:
  - property: voltage
    note: battery voltage is only available with custom firmware
  - property: rssi
    note: >
      The RSSI sensor is disabled by default. You can enable the RSSI sensor by going to `configuration`, `integrations`, select `devices` on the BLE monitor integration tile and select your device. Click on the `+1 disabled entity` to show the disabled sensor and select the disabled entity. Finally, click on `Enable entity` to enable it. 
broadcast_rate: "1/10min. (battery level 1/hr.)"
active_scan:
encryption_key: true
custom_firmware:
  - name: pvvx
    url: https://github.com/pvvx/ATC_MiThermometer
notes:
  - Custom firmware's broadcast temperature, humidity, battery voltage and battery level in percent. Broadcast interval can be set by the user and encryption can be used as an option. BLE monitor will automatically use the advertisement type with the highest accuracy, when setting the firmware to broadcast all advertisement types.
---
