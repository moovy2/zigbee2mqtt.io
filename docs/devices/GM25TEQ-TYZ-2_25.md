---
title: "Moes GM25TEQ-TYZ-2/25 control via MQTT"
description: "Integrate your Moes GM25TEQ-TYZ-2/25 via Zigbee2MQTT with whatever smart home infrastructure you are using without the vendor's bridge or gateway."
addedAt: 2025-08-01T15:19:08
pageClass: device-page
---

<!-- !!!! -->
<!-- ATTENTION: This file is auto-generated through docgen! -->
<!-- You can only edit the "Notes"-Section between the two comment lines "Notes BEGIN" and "Notes END". -->
<!-- Do not use h1 or h2 heading within "## Notes"-Section. -->
<!-- !!!! -->

# Moes GM25TEQ-TYZ-2/25

|     |     |
|-----|-----|
| Model | GM25TEQ-TYZ-2/25  |
| Vendor  | [Moes](/supported-devices/#v=Moes)  |
| Description | Roller Shade Blinds Motor for 38mm Tube |
| Exposes | cover (state, position), motor_direction |
| Picture | ![Moes GM25TEQ-TYZ-2/25](https://www.zigbee2mqtt.io/images/devices/GM25TEQ-TYZ-2-25.png) |


<!-- Notes BEGIN: You can edit here. Add "## Notes" headline if not already present. -->


<!-- Notes END: Do not edit below this line -->




## Exposes

### Cover 
The current state of this cover is in the published state under the `state` property (value is `OPEN` or `CLOSE`).
To control this cover publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"state": "OPEN"}`, `{"state": "CLOSE"}`, `{"state": "STOP"}`.
It's not possible to read (`/get`) this value.
To change the position publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"position": VALUE}` where `VALUE` is a number between `0` and `100`.

### Motor direction (enum)
Set the motor direction.
Value can be found in the published state on the `motor_direction` property.
It's not possible to read (`/get`) this value.
To write (`/set`) a value publish a message to topic `zigbee2mqtt/FRIENDLY_NAME/set` with payload `{"motor_direction": NEW_VALUE}`.
The possible values are: `forward`, `back`.

