---
description: >-
  You can easily get the state of LEDs on top of the screen by using this
  command
---

# 💡 Get leds state

## Command

```javascript
GET_LEDS_STATE
```

### Arguments

There are no arguments for this function.

## Response

The response of this command is :

```javascript
RESPONSE:GET_LEDS_STATE;<STATE>
```

### Arguments

| Argument name | Type | Possibilities |
| ------------- | ---- | ------------- |
| STATE         | bool | 0 or 1        |

## Examples

### Get the current LEDs state

```javascript
GET_LEDS_STATE
```
