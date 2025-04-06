---
description: >-
  You can easily control the state of LEDs on top of the screen (shut them
  off/turn them on) by using this command
---

# 💡 Set leds state

## Command

```javascript
SET_LEDS_STATE:<STATE>
```

## Arguments

| Argument name | Type | Possibilities |
| ------------- | ---- | ------------- |
| STATE         | BOOL | 0 or 1        |

## Examples

### Turn the LEDs on

```javascript
SET_LEDS_STATE:1
```

### Turn the LEDs off

```javascript
SET_LEDS_STATE:0
```
