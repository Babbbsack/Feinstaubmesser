# Feinstaubmesser
## 1. Beschreibung
Nach einem DLF-Podcast stellt Feinstaub ein sehr hoher Gesundheitsrisiko dar.
Mit einem Arduino Messsystem könnte man sich an Messung für Internet (Citizenscience) beteiligen oder testweise mal Luft in Kau (Schrottplatz und Landstraße), Stadtallendorf (Winter, Ferrero), Innenraum bei unserem Dieselmotor, Rasenmäher und Kamin testen

https://sensor.community/de/

https://blog.helmutkarger.de/category/projekte/feinstaubsensor/page/2/


Gemäß diesem Paper (https://www.nature.com/articles/s41586-021-04134-6) und dem entsprechenden DLF-Beitrag sind Organophosphate (Zerfallsprodukte von Branschutzmitteln in diversen Gegenständen) überall in Luft in Großstädten vorhanden. Auswirkungen auf Gesundheit sind noch nicht bekannt.

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
