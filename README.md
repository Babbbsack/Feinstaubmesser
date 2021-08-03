# Feinstaubmesser
## 1. Beschreibung
https://sensor.community/de/

https://blog.helmutkarger.de/category/projekte/feinstaubsensor/page/2/


## 2. Teileliste
* Teil 1
* Teil 2

## 3. Meine Umsetzung/Wichtige Links/Codes
*Formatierung von Text in github:*

*https://www.heise.de/tipps-tricks/GitHub-Seiten-mit-Markdown-gestalten-4575536.html*

**Inbetriebnahme eines neues Raspberries:**

* **Aktivierung von WLan:**

*Auf der Boot-Partition im Rootverzeichnis wird eine leere Datei mit dem Namen "wpa_supplicant.conf" erstellt und je nach Version des Betriebssystems Raspian mit unterschiedlichen Daten gefüllt. Hier werden die beiden Werte ssid und psk jeweils durch die entsprechenden individuellen Angaben angepasst.*

    country=DE
    ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
    update_config=1
    network={
    ssid="wlan-ssid"
    psk="wlan-passwort"
    key_mgmt=WPA-PSK
    }

* **Einrichtung automatischer Updates von Debian:**

*https://stqu.de/joomla/de/raspberry-pi/90-pi-automatische-updates-unattended-upgrades*

* **Zugriff auf Konsole:**

*SSH-Aktivierung (leere Datei "SSH" ohne Endung mit auf SD-Karte ablegen) und Putty kann man sich vom PC auf Raspberry verbinden und muss nicht immer Laptop über Kabel verbinden:*

* **Zugriff auf Desktop:**

*Siehe Schritt 3 (http://www.technik-tipps-und-tricks.de/raspberry-pi/raspberry-pi-konfigurieren/). Anschlißend in Windows über "Remotedesktopverbindung" eine Verbindung über die IP des Gerätes herstellen*


## 4. Überlegungen für spätere Optimierungen
