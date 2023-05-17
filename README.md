# Entry-M_TempHumidityMonitor
Using Arduino Uno as host, display temperature and humidity on Entry-M / M-Series display.

What you need:
	Arduino (Uno here. Any other types are also fine).
	Entry-M or M-series display from Winstar. (e.g. WL0F00043000UNFAAEA00)
	DHT11 temperature/humidity sensor (DHT22 is ok).
	Power adapters for arduino and display.
	Others: 
		USB cable
		Wires
		UART(NOT RS232 NOR RS485) adapter, if you want to monitor UART commands.
	
Material:
	A 480 x 272 image for background (Loaded to background layer)
	Load a custom font you like (We load Russo One 36 Regular here)
	
Connection:
	DHT11 GND to GND, Vcc to 5V, Vout to Arduino pin 2.
	DHT11 Vout should be pull-up to 5V (5k or 10k register is ok).
	Display GND to GND, Vcc to 5V.
	Arduino Pin 1 (Tx) to display Rx, Pin 0 to display Tx.
	If you want to connect more than one display together, please connect only only one Tx of the displays to the Rx of Arduino.
	