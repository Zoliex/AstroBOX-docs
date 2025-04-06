---
description: >-
  Every time the GPS will send data to the microcontroller, you'll receive this
  event in the serial
---

# 🌍 GPS position

## Event

```javascript
GPS:<LAT>;<LON>;<ALT>;<SATS>;<DATETIME>
```

## Arguments

| Argument name | Description                        | Type  |
| ------------- | ---------------------------------- | ----- |
| LAT           | Latitude (in deg)                  | float |
| LON           | Longitude (in deg)                 | float |
| ALT           | Altitude (in m)                    | float |
| SATS          | Current connected satellites       | int   |
| DATETIME      | Unix current date and time (GMT+0) | date  |
|               |                                    |       |

## Examples

## A frame sent by a GPS located in Paris on 6 April 2024 at 13h 01 min 45s with 8 satellites connected and at an altitude of 35.1m

```javascript
GPS:48.866667;2.333333;35.1;8;1743937305
```
