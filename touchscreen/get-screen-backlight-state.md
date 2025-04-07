---
description: >-
  You can easily get the state of the backlight of the screen by using this
  command
---

# 💻 Get screen backlight state

## Command

```javascript
GET_BACKLIGHT_STATE
```

### Arguments

There are no arguments for this command.

## Response

The response of this command is :

```javascript
RESPONSE:GET_BACKLIGHT_STATE;<STATE>
```

### Arguments

| Argument name | Type | Possibilities |
| ------------- | ---- | ------------- |
| STATE         | bool | 0 or 1        |

## Examples

### Get the current backlight state

```javascript
GET_BACKLIGHT_STATE
```
