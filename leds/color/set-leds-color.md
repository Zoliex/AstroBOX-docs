---
description: >-
  Set the current color of LEDs (with fade between new color and old color). The
  new color must be sent as an RGB 8bit value.
---

# 💡 Set leds color

## Command

```javascript
SET_LEDS_COLOR:<RED>;<GREEN>;<BLUE>
```

### Arguments

| Argument name | Type | Possibilities |
| ------------- | ---- | ------------- |
| RED           | int  | 0-255         |
| GREEN         | int  | 0-255         |
| BLUE          | int  | 0-255         |

## Response

The response of this command is :

```javascript
RESPONSE:SET_LEDS_COLOR;<RED>;<GREEN>;<BLUE>
```

### Arguments

| Argument name | Type | Possibilities |
| ------------- | ---- | ------------- |
| RED           | int  | 0-255         |
| GREEN         | int  | 0-255         |
| BLUE          | int  | 0-255         |

## Examples

### Turn the LEDs red

```javascript
SET_LEDS_COLOR:255;0;0
```

### Turn the LEDs orange

```javascript
SET_LEDS_COLOR:255;128;0
```
