---
description: >-
  You can set the fan speed of the box by sending the command to the
  microcontroller
---

# 💨 Set fan speed

## Command

```javascript
SET_FAN_SPEED:<SPEED>
```

### Arguments

| Argument name | Type | Possibilities |
| ------------- | ---- | ------------- |
| SPEED         | int  | 0%-100%       |

## Response

The response of this command is :

```javascript
RESPONSE:SET_FAN_SPEED;<SPEED>
```

### Arguments

| Argument name | Type | Possibilities |
| ------------- | ---- | ------------- |
| SPEED         | int  | 0%-100%       |

## Examples

### Set the fan speed at 50%

```javascript
SET_FAN_SPEED:50
```

