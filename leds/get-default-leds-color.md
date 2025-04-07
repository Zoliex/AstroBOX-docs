---
description: Get the default color of LEDs at startup.
---

# 💡 Get default leds color

## Command

```javascript
GET_DEFAULT_LEDS_COLOR
```

### Arguments

There are no argument for this function.

## Response

The response of this command is :

```javascript
RESPONSE:GET_DEFAULT_LEDS_COLOR;<RED>;<GREEN>;<BLUE>
```

### Arguments

| Argument name | Type | Possibilities |
| ------------- | ---- | ------------- |
| RED           | int  | 0-255         |
| GREEN         | int  | 0-255         |
| BLUE          | int  | 0-255         |

## Examples

### Get the default LEDs color

```javascript
GET_DEFAULT_LEDS_COLOR
```
