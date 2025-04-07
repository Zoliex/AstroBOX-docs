---
description: >-
  You can set the default fan speed at startup of the box by sending the command
  to the microcontroller. The speed will not change directly using this command.
---

# 💨 Set default fan speed

## Command

```javascript
SET_DEFAULT_FAN_SPEED:<SPEED>
```

### Arguments

| Argument name | Type | Possibilities |
| ------------- | ---- | ------------- |
| SPEED         | int  | 0%-100%       |

## Response

The response of this command is :

```javascript
RESPONSE:SET_DEFAULT_FAN_SPEED;<SPEED>
```

### Arguments

| Argument name | Type | Possibilities |
| ------------- | ---- | ------------- |
| SPEED         | int  | 0%-100%       |

## Examples

### Set the default fan speed at 50%

```javascript
SET_DEFAULT_FAN_SPEED:50
```

