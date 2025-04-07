---
description: >-
  You can get the default fan speed at startup of the box by sending the command
  to the microcontroller.
---

# 💨 Get default fan speed

## Command

```javascript
GET_DEFAULT_FAN_SPEED
```

### Arguments

There are no argument for this command.

## Response

The response of this command is :

```javascript
RESPONSE:GET_DEFAULT_FAN_SPEED;<SPEED>
```

### Arguments

| Argument name | Type | Possibilities |
| ------------- | ---- | ------------- |
| SPEED         | int  | 0%-100%       |

## Examples

### Get the default fan speed

```javascript
GET_DEFAULT_FAN_SPEED
```

