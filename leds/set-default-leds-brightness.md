---
description: >-
  You can easily set the default startup brightness of LEDs on top of the screen
  by using this command. The brightness will not change using this command.
---

# 💡 Set default leds brightness

## Command

```javascript
SET_DEFAULT_LEDS_BRIGHTNESS:<BRIGHTNESS>
```

### Arguments

| Argument name | Type | Possibilities |
| ------------- | ---- | ------------- |
| BRIGHTNESS    | int  | 0%-100%       |

## Response

The response of this command is :

```javascript
RESPONSE:SET_DEFAULT_LEDS_BRIGHTNESS;<BRIGHTNESS>
```

### Arguments

| Argument name | Type | Possibilities |
| ------------- | ---- | ------------- |
| BRIGHTNESS    | int  | 0%-100%       |

## Examples

### Set the default LEDs brightness at 50%

<pre class="language-javascript"><code class="lang-javascript"><strong>SET_DEFAULT_LEDS_BRIGHTNESS:50
</strong></code></pre>

