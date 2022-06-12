# temp_sensor: A basic temperature logger

On initial power up, sets up a serial connection over USB.
Immediately starts logging temperature data to SD card, using current time.
Updates temperature data every minute.
Only appends to the data file.
If serial connection from USB sends new date/time, that updates clock.

# Bill of materials

* Arduino Nano
* 9V battery connector
* Temperature sensor [https://www.amazon.com/Adafruit-MCP9808-Accuracy-Temperature-Breakout/dp/B00OKCQX96]
* SD card interface [https://www.amazon.com/HiLetgo-Adater-Interface-Conversion-Arduino/dp/B07BJ2P6X6]
* Clock module [https://www.amazon.com/dp/B082VL4GM6]
* Some kind of enclosure

# Data format

Basic CSV file with columns:
1. Year
2. Month
3. Day
4. Hour
5. Minute
6. Second
7. Temperature