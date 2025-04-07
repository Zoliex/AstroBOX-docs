---
description: >-
  You can easily control the state of the backlight of the screen (shut it
  off/turn it on) by using this command
---

# 💻 Set screen backlight state

## Command

```javascript
SET_BACKLIGHT_STATE:<STATE>
```

### Arguments

| Argument name | Type | Possibilities |
| ------------- | ---- | ------------- |
| STATE         | BOOL | 0 or 1        |

## Response

The response of this command is :

```javascript
RESPONSE:SET_BACKLIGHT_STATE;<STATE>
```

### Arguments

| Argument name | Type | Possibilities |
| ------------- | ---- | ------------- |
| STATE         | bool | 0 or 1        |

## Examples

### Turn the screen backlight on

```javascript
SET_BACKLIGHT_STATE:1
```

### Turn the screen backlight off

```javascript
SET_BACKLIGHT_STATE:0
```
