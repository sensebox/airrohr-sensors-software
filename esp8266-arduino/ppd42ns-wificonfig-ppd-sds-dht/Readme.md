Version für Sensoren PPD42NS, SDS011 und DHT22. Inklusive Konfiguration über WLAN.

Grundsätzliche Konfiguration der Parameter über die Datei ext_dev.h .

WLAN Konfiguration:

Wenn das vorgegebene WLAN nach 10 Sekunden nicht erreichbar ist, wird ein Access-Point eingerichtet, der über "Feinstaubsensor-\[Sensor-ID\]" erreichbar ist. Nach dem Verbinden zu diesem Accesspoint werden alle Anfragen auf die Konfigurationsseite umgeleitet.

Konfigurierbar sind:
- WLAN-Name und Passwort
- welche Sensoren sollen ausgelesen werden
- an wen werden die Daten gesendet

Nach 5 Minuten wird der Access-Point wieder deaktiviert.

  
  
Benötigte Software:
Arduino IDE <https://www.arduino.cc/en/Main/Software>  
ESP8266 für Arduino <http://arduino.esp8266.com/stable/package_esp8266com_index.json>  

  
Verwendete Bibliotheken:  
  
DHT <https://github.com/adafruit/DHT-sensor-library>  
(DHT.cpp und DHT.h downloaden und in das Softwareverzeichnis kopieren)  
SoftwareSerial <https://github.com/plerup/espsoftwareserial>  
WifiManager <https://github.com/tzapu/WiFiManager>  
  
In ESP8266 für Arduino IDE enthalten:  
FS  
ESP8266WiFi  
ESP8266WebServer  
DNSServer  
  
In Arduino IDE enthalten:
ArduinoJson  