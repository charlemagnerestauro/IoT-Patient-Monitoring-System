> Materials:

 - MAX30100 Pulse Oximeter Sensor
 - DHT22 Temperature and Humidity Sensor
 - DS18B20 Temperature Sensor
 - Esp32 with development board
 - 0.96 inch oled display
 - Active Buzzer
 - Resistors (220 ohms, 4.7k ohms, 10k ohms)
 - LED

> Assemble parts shown in circuit_image.png, or

> read IoT_Patient_Monitor_Schematic.pdf

> download following libraries in Arduino IDE

 - MAX30100_PulseOximeter.h
 - DHT.h
 - OneWire.h
 - DallasTemperature.h
 - Adafruit_GFX.h
 - Adafruit_SSD1306.h

> Upload code given: code used.txt

> set-up blynk dashboard in blynk web browser at blynk.io


------------Blynk Set-up------------

> developer zone 
> create new template 
> add datastreams
 set: 
  - V1 - Room Temp - degCelsius
  - V2 - Room Humidity - %
  - V3 - Body Temp - degCelsius
  - V4 - Heart rate ave - bpm
  - V5 - Oxygen Level - %
> save

> go to 'web dashboard'
> add gauge, displays, etc.
> assign to each datastream 
> save


> go to 'events and notifications'
> add new event
> 

event name: High Heart Rate Alert, event code: hr_alert
event name: Fever Alert, event code: fever_alert

> go to 'notification' and turn it on
> on: Push notifications and email to device owner
> Enable notifications management, Deliver push notifications as alerts
> save

> exit developer zone
> go to devices
> add new device: from created template.

> optional: create mobile dashboard by downloading blynk app 

-------------------------------------------------------------

> make sure all connections are correct

> change WIFi SSID and Password

> upload the sketch to the esp32

> wait for blynk iot to connect






