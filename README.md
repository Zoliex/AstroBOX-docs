---
description: Everything you need to know to start sending commands to AstroBox
---

# 👑 Get started

AstroBOX is a powerful ESP8266-based module that enables interaction with hardware components such as screens, LEDs, GPS modules, and touch sensors. Communication with AstroBOX is done via a serial interface using a baudrate of **115200**.

This guide will walk you through the setup process and explain how to send and receive commands to/from AstroBOX.

***

### 🛠️ Requirements

* A computer (Windows/macOS/Linux)
* A USB-to-Serial adapter or a direct USB connection to AstroBOX
* A terminal program (e.g., [PuTTY](https://www.putty.org/), CoolTerm, MobaXTerm, or Arduino Serial Monitor from Arduino IDE)
* AstroBOX firmware installed on the ESP8266
* Serial baudrate: **115200**

***

### 🔌 Connecting to AstroBOX

1. **Connect AstroBOX via USB**\
   Use a USB cable or serial adapter to connect AstroBOX to your computer.
2. **Open your terminal program**
   * Set the **baudrate** to `115200`
   * Use **8 data bits**, **no parity**, **1 stop bit** (8N1)
   * Disable hardware and software flow control
3. **Start communicating!**

***

### 📡 Communication Protocol Overview

AstroBOX uses a simple ASCII-based command protocol over serial. All commands are terminated by a newline character : `\n`.

#### 🔄 Keep-Alive System

AstroBOX requires a `KEEP_ALIVE` command to be sent **every second** to remain in **remote control mode**. If the keep-alive signal is not received within 3 seconds, it will enter **manual mode**, allowing local control via buttons or touch screen.

**KEEP\_ALIVE command:**

```
KEEP_ALIVE
```

You must automate this in your software to ensure uninterrupted communication.

***

### 📤 Sending Commands to AstroBOX

Here are some example commands you can send:

| Command                               | Description                              |
| ------------------------------------- | ---------------------------------------- |
| `TOGGLE_BACKLIGHT_STATE`              | Toggle screen backlight                  |
| `SET_LEDS_COLOR:<RED>;<GREEN>;<BLUE>` | Set LED color to RGB values (0-255 each) |
| `SET_FAN_SPEED:<SPEED>`               | Set fan speed (in %)                     |

All commands must be terminated with `\n`.

***

### 📥 Receiving Commands from AstroBOX

AstroBOX can also **send information** via serial, such as:

| Message                                   | Description                               |
| ----------------------------------------- | ----------------------------------------- |
| `GPS:<LAT>;<LON>;<ALT>;<SATS>;<DATETIME>` | Current GPS coordinates                   |
| `TOUCH_CLICK:<POS_X>;<POS_Y>;<POS_Z>`     | Touch screen event at coordinates (X,Y,Z) |

Your software should parse these messages line-by-line to process the data (use `\n` or `\r` as carriage return).

***

### 🧪 Example Session

Here's what a session might look like in practice:

```
TOUCH_CLICK:2329;2122;1104
TOUCH_RELEASE:2322;2081;902
```

***

### ⚠️ Important Notes

* You **must send `KEEP_ALIVE` every second** or AstroBOX will stop listening to commands and switch to manual mode.
* Each command should be sent as a full line ( terminated).
* Avoid sending malformed or partial commands, as they may be ignored.

***

### ✅ Best Practices

* Use a timer in your code to send `KEEP_ALIVE` regularly.
* Always parse incoming messages line-by-line.
* Buffer and retry commands if the serial link is temporarily busy.

***

### 🧩 Integrating with Your Application

You can easily integrate AstroBOX into your custom application using any programming language that supports serial communication (e.g., Python, C#, Node.js, C++).

For example, in Python (using `pyserial`):

```python
import serial
import time

ser = serial.Serial('COM3', 115200, timeout=1)

def send_keep_alive():
    ser.write(b'KEEP_ALIVE\n')

while True:
    send_keep_alive()
    time.sleep(1)
```

***

### 💬 Questions or Issues?

If you're having trouble communicating with AstroBOX, check the following:

* Is the baudrate set to 115200?
* Are commands correctly terminated with `\n` or `\r` ?
* Are you sending `KEEP_ALIVE` every second?
