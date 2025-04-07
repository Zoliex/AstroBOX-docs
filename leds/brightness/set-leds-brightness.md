---
description: >-
  You can easily control the brightness of LEDs on top of the screen by using
  this command
---

# 💡 Set leds brightness

## Command

```javascript
SET_LEDS_BRIGHTNESS:<BRIGHTNESS>
```

### Arguments

| Argument name | Type | Possibilities |
| ------------- | ---- | ------------- |
| BRIGHTNESS    | int  | 0%-100%       |

## Response

The response of this command is :

```javascript
RESPONSE:SET_LEDS_BRIGHTNESS;<BRIGHTNESS>
```

### Arguments

| Argument name | Type | Possibilities |
| ------------- | ---- | ------------- |
| BRIGHTNESS    | int  | 0%-100%       |

## Examples

### Set the LEDs brightness at 50%

<pre class="language-javascript"><code class="lang-javascript"><strong>SET_LEDS_BRIGHTNESS:50
</strong></code></pre>

