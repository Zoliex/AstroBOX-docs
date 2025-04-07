---
description: >-
  You can get the fan speed of the box by sending the command to the
  microcontroller
---

# 💨 Get fan speed

## Command

```javascript
GET_FAN_SPEED
```

### Arguments

There are no arguments for this command.

## Response

The response of this command is :

```javascript
RESPONSE:GET_FAN_SPEED;<SPEED>
```

### Arguments

| Argument name | Type | Possibilities |
| ------------- | ---- | ------------- |
| SPEED         | int  | 0%-100%       |

## Examples

### Get the current fan speed

```javascript
GET_FAN_SPEED
```
