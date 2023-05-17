# Temperature and Humidity Monitor
Using Arduino Uno as host, display temperature and humidity on Entry-M / M-Series display.

### What you need
- Arduino (Uno here. Any other types are also fine).
- Entry-M or M-series display from Winstar. (e.g. WL0F00043000UNFAAEA00)
- DHT11 temperature/humidity sensor (DHT22 is ok).
- Power adapters for arduino and display.
- USB cable
- Wires
- UART(NOT RS232 NOR RS485) adapter, if you want to monitor UART commands.

### Material
- A 480 x 272 image for background (Loaded to background layer)
- Load a custom font you like (We load Russo One 36 Regular here)

### Connection
#####  DHT11
- GND to GND, Vcc to 5V
- Vout connected to pin 2 of Arduino.
- Vout should be pull-up to 5V (5k or 10k register is ok).

##### Display
- GND to GND, Vcc to 5V.
- Rx connected to the Tx of Arduino
- Tx connected to the Rx of Arduino

##### Multi-Display
If you want to display on more than one display simultaneously, please connect only one Tx of the displays to the Rx of Arduino.
