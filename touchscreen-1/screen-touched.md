---
description: Every time the user touch the screen, this event is fired
---

# 💻 Screen touched

## Event

```javascript
TOUCH_CLICK:<POS_X>;<POS_Y>;<POS_Z>
```

## Arguments

| Argument name | Description                 | Type | Possibilities |
| ------------- | --------------------------- | ---- | ------------- |
| POS\_X        | Touch X position            | int  | 0-4096        |
| POS\_Y        | Touch Y position            | int  | 0-4096        |
| POS\_Z        | Touch Z position (pressure) | int  | 0-4096        |

## Examples

### A simple touch

```javascript
TOUCH_CLICK:2580;3563;1584
```
