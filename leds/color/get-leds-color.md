---
description: Get the current color of the LEDs.
---

# 💡 Get leds color

## Command

```javascript
GET_LEDS_COLOR
```

### Arguments

There is no argument for this function.

## Response

The response of this command is :

```javascript
RESPONSE:GET_LEDS_COLOR;<RED>;<GREEN>;<BLUE>
```

### Arguments

| Argument name | Type | Possibilities |
| ------------- | ---- | ------------- |
| RED           | int  | 0-255         |
| GREEN         | int  | 0-255         |
| BLUE          | int  | 0-255         |

## Examples

### Get the LEDs color

```javascript
GET_LEDS_COLOR
```
