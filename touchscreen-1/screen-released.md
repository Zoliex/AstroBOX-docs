---
description: Every time the user release the screen, this event is fired
---

# 💻 Screen released

## Event

```javascript
TOUCH_RELEASE:<POS_X>;<POS_Y>;<POS_Z>
```

### Arguments

| Argument name | Description                   | Type | Possibilities |
| ------------- | ----------------------------- | ---- | ------------- |
| POS\_X        | Release X position            | int  | 0-4096        |
| POS\_Y        | Release Y position            | int  | 0-4096        |
| POS\_Z        | Release Z position (pressure) | int  | 0-4096        |

## Examples

### A simple release

```javascript
TOUCH_RELEASE:2667;3529;970
```
