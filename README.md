# raspberry_solarreader
Solarreader_fuer_RaspberryPi
Beschreibung:
lauffähig ab Raspberry Pi2B+  , auch Grafana, dort mit USB-Wlan-Adapter oder LAN, 
Mit Hilfestellung ist auch Betrieb über USB möglich.

ab Pi3B+ ist Wlan  und USB-Start über OS integriert

Basis: Compatible with:

    All Raspberry Pi models

Raspberry Pi OS with desktop

    Release date: Mai 2021 
    System: 32-bit
    Kernel version: 5.10
    Debian version: 10 (buster)
    Relase 1,2G
       Release notes mit aktuell verfügbaren updates ausgestattet


-   influx V.1.8.10, 
-   java -version (openjdk version "11.0.18" 2023-01-17),
-   Grafana 9.3.2,
-   MQTT (Mosquitto)
-   Browser Chromium & Mozilla Firefox ESR
-   Apache2 
-   PHP7.34 für individuellen Gebrauch
-   Raspberry_Handbuch_Deutsch

-   6 InfluxDB,  solaranzeige, steuerung, solarreader, solarreader1, solarreader2, solarreader3
-   alle angelegt und in Grafana bekannt gemacht,
-   müssen nur in der Konfigurations-GUI aktiviert werden.

- Datensicherung der influxDB‘s bereits vorbereitet. 
- Alle Grafana-Stanbdard-Dashboards der solaranzeige enthalten.
- Passwörter:

- Raspberry: user: pi,   Passwort: solarreader
- Grafana: user: admin   Passwort: solarreader

-Download mit

  https://solarfanenrico.de/solarreader/solarreader_1_3_raspberry_2023-02-17.img.zip  (aktuell)


entpacken und auf microSD ein Laufwerksabbild erstellen
in den Pi stecken und starten
den komplettesn Speicher freigeben mit

sudo raspi-config

6 Advanced Options    auswählen

danach

A1 Expanded Filesystem     wählen

dadurch bereitet sich der Pi auf die neue Laufwerksgröße vor.
Den Pi automatisch starten lassen

mit dem Konsolenbefehl

df -h kann man den Erfolg kontrollieren
bei einer 15 GB SD sieht die erste Antwortzeile so aus
Dateisystem Größe Benutzt Verf. Verw% Eingehängt auf
/dev/root        15G    5,6G    8,1G   41%        /

in einem beliebigen Browser auf einem beliebigen Grerät

die IP des Rasperrys eintragen. Es folgt dr Hinweis
mit IP des RaspberryPI:8080 wird die Konfigurationsoberfläche aufgerufen
und 
Grafana mit IP des Raspberry:3000

die erweiterte Anleitung gibt es als PDF unter

https://solarfanenrico.de/Solarreader_Installation.pdf 

diese ist zwar noch nicht endgültig fertig, weil ich selbst auch noch nicht alle Möglichkeiten nutze.
Hier bin ich auf die Zuarbeit von Euch angewiesen.

Gebt Vorschläge, damit es verbessert werden kann
