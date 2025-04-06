---
description: >-
  Every time the user touch the screen from more than 5 seconds, this event is
  fired
---

# 💻 Screen touched >5s

## Event

```javascript
TOUCH_LONG_CLICK:<POS_X>;<POS_Y>;<POS_Z>
```

## Arguments

| Argument name | Description                      | Type | Possibilities |
| ------------- | -------------------------------- | ---- | ------------- |
| POS\_X        | Long touch X position            | int  | 0-4096        |
| POS\_Y        | Long touch Y position            | int  | 0-4096        |
| POS\_Z        | Long touch Z position (pressure) | int  | 0-4096        |

## Examples

### A simple long touch

```javascript
TOUCH_LONG_CLICK:841;2157;2133
```
