<img width="320px" src="assets/logo-w-400.png" align="left"/>

<br><br><br>

[![Current Release](https://img.shields.io/github/release/hobbyquaker/RedMatic.svg?colorB=4cc61e)](https://github.com/hobbyquaker/RedMatic/releases/latest)
[![Dependencies Status](https://david-dm.org/hobbyquaker/redmatic/status.svg)](https://david-dm.org/hobbyquaker/redmatic)
[![Build Status](https://travis-ci.org/hobbyquaker/RedMatic.svg?branch=master)](https://travis-ci.org/hobbyquaker/RedMatic)

[Node-RED](https://nodered.org/about/) als Addon für die 
[Homematic CCU3](https://www.eq-3.de/produkte/homematic/zentralen-und-gateways/smart-home-zentrale-ccu3.html) und 
[RaspberryMatic](https://github.com/jens-maus/RaspberryMatic)

<br>

_RedMatic_ fasst mehrere Softwarekomponenten zu einem CCU Addon zusammen, einem Softwarepaket, dass auf einer Homematic 
CCU3 oder RaspberryMatic als Zusatzsoftware komfortabel über das WebUI installiert werden kann.

Die Grundlage bildet [Node-RED](https://nodered.org/about/) mit den 
[CCU Nodes für Node-RED](https://github.com/hobbyquaker/node-red-contrib-ccu). Hiermit ist es auf einfache, visuelle 
Weise möglich Regeln, Automationen, Scripte und Anbindungen von externen Services und Systemen für ein Homematic System 
zu realisieren - und das weitgehend auch ohne Programmierkenntnisse. Im 
[Wiki](https://github.com/hobbyquaker/RedMatic/wiki) gibt es weitere Informationen zu Node-RED und einige 
Anwendungsbeispiele (sogenannte _Flows_).

Außerdem ist die Node-RED Erweiterung [Node-RED Dashboard](https://github.com/node-red/node-red-dashboard) enthalten, 
mit der ansprechende User Interfaces für Mobilgeräte und den Browser erstellt werden können
([Beispiel Screenshots](https://github.com/hobbyquaker/RedMatic/wiki/Dashboard-Screenshots)).

_RedMatic_ ist __nur für die CCU3 und RaspberryMatic geeignet__. Auf der CCU2 kann es nicht verwendet werden.

Für die Nutzung der CCU Nodes ist ein moderner Browser notwendig, der Internet Explorer wird nicht unterstützt.


## Schnellstart

Unter [Releases](https://github.com/hobbyquaker/RedMatic/releases/latest) steht die Datei `redmatic-<version>.tar.gz` 
zum Download zur Verfügung. Nach der Installation des Addons über das Homematic WebUI (Systemsteuerung -> 
Zusatzsoftware) und dem darauf folgenden Reboot der CCU ist Node-RED unter `http://<ccu-addresse>/addons/red` 
erreichbar. Bei der Installation ist Geduld erforderlich, es kann bis zu ~10 Minuten dauern. Einige Beispiel-Flows sowie
ein einfaches Dashboard sind bereits vorkonfiguriert, das Dashboard ist unter `http://<ccu-addresse>/addons/red/ui` 
erreichbar.


## Support, Mitarbeit

Für Feedback jeglicher Art, Fragen, Vorschläge, Wünsche und Fehlerberichte bitte den 
[Issue Tracker](https://github.com/hobbyquaker/RedMatic/issues) nutzen. Alternativ steht auch 
[Slack](https://join.slack.com/t/homematicuser/shared_invite/enQtNDE2MjAwOTI0OTgzLWNmMzIzMTZlZWYxMWU0MWJiY2NmMWQ0NWQ2MDViMjllN2M5ZTMxMTZjNmIxNTlkZTRhMTExM2I2ZDJjN2M3ZjU) 
zur Verfügung. 

Beteiligung in jeder Form ist willkommen und gewünscht, insbesondere sind alle Nutzer aufgefordert die [Liste erfolgreich getesteter Nodes](https://github.com/hobbyquaker/RedMatic/wiki/Erfolgreich-getestete-Nodes) zu ergänzen, Beispiel-Flows zu veröffentlichen und an der Verbesserung und Erweiterung der [Dokumentation](https://github.com/hobbyquaker/RedMatic/wiki) mitzuarbeiten.

Es werden keine Spenden angenommen, ich würde mich jedoch darüber freuen wenn der erfolgreiche Einsatz dieser Software mit einem Github Sternchen ⭐️ honoriert wird (Github Account ist schnell angelegt! ;-)


## Dokumentation

* Administration
  * [Installation](https://github.com/hobbyquaker/RedMatic/wiki/Installation)
  * [Update](https://github.com/hobbyquaker/RedMatic/wiki/Update)
  * [Deinstallation](https://github.com/hobbyquaker/RedMatic/wiki/Deinstallation)
  * [Zusätzliche Nodes installieren](https://github.com/hobbyquaker/RedMatic/wiki/Node-Installation)
  * [Erfolgreich mit RedMatic getestete Nodes](https://github.com/hobbyquaker/RedMatic/wiki/Erfolgreich-getestete-Nodes) - bitte diese Liste ergänzen!
  * [Log-Level erhöhen für Fehleranalyse](https://github.com/hobbyquaker/RedMatic/wiki/Loglevel)
  * [Passwort Schutz für Node-RED einrichten](https://github.com/hobbyquaker/RedMatic/wiki/Passwort)
* Nutzung
  * [Node-RED Grundlagen](https://github.com/hobbyquaker/RedMatic/wiki/Node-RED)
  * [CCU Nodes](https://github.com/hobbyquaker/RedMatic/wiki/CCU-Nodes)
  * [Tipps](https://github.com/hobbyquaker/RedMatic/wiki/Tipps)
  * [Flows exportieren](https://github.com/hobbyquaker/RedMatic/wiki/Flow-Export)
* Beispiel Flows
  * [Anzahl und Liste offener Fenster im Dashboard anzeigen](https://github.com/hobbyquaker/RedMatic/wiki/Flow-Windows)
  * [Hue Lampen mit langem Tastendruck dimmen](https://github.com/hobbyquaker/RedMatic/wiki/Flow-Hue)
  * [UNREACH Meldung unterdrücken](https://github.com/hobbyquaker/RedMatic/wiki/Flow-Unreach)
  * [Anzeigen und Setzen von Systemvariablen im Dashboard](https://github.com/hobbyquaker/RedMatic/wiki/Flow-Sysvar-Dashboard)
  * [DutyCycle Graph im Dashboard anzeigen](https://github.com/hobbyquaker/RedMatic/wiki/Flow-DutyCycle)
  * [Per Pushover benachrichtigen wenn Fenster länger als 10 Minuten offen ist](https://github.com/hobbyquaker/RedMatic/wiki/Flow-Window-Pushover)
  * [CPU Auslastung als Graph im Dashboard anzeigen](https://github.com/hobbyquaker/RedMatic/wiki/Flow-CPU-Usage)
  * [JSON Daten von Webservice abfragen und in Systemvariable schreiben](https://github.com/hobbyquaker/RedMatic/wiki/Flow-HTTP-Client)
  * [Inhalt einer Systemvariablen über einfachen Webservice bereitstellen](https://github.com/hobbyquaker/RedMatic/wiki/Flow-HTTP-Server)
  * [Schnelles Blinken der LED im Offline-Betrieb unterbinden](https://github.com/hobbyquaker/RedMatic/wiki/Flow-Offline-LED)
  * [CCU an MQTT anbinden](https://github.com/hobbyquaker/RedMatic/wiki/Flow-MQTT)
* Von Usern bereitgestellte Flows
  * [Licht mittels Tastendruck aus und einschalten](https://github.com/hobbyquaker/RedMatic/wiki/Flow-simple-toggle-light)
  * [Textausgabe mittels Chromecast oder Google Home](https://github.com/hobbyquaker/RedMatic/wiki/Flow-speak-text-on-Google)
  * [Berechnung von Feiertagen](https://github.com/hobbyquaker/RedMatic/wiki/Flow-to-calculate-german-holidays)
  * [Funktion nur innerhalb einer bestimmten Uhr-Zeit ausführen](https://github.com/hobbyquaker/RedMatic/wiki/Flow-within-time)
  * [Fehlerüberwachung der CCU](https://github.com/hobbyquaker/RedMatic/wiki/Flow-Syslog)
  * [Integration Weatherman (JSON, httpStatic, SteelSeries Gauges)](https://github.com/hobbyquaker/RedMatic/wiki/https://github.com/Sineos/node-red-contrib-weatherman/blob/master/README_DE.md)
  * [Systeminformationen der CCU Zentrale](https://github.com/hobbyquaker/RedMatic/wiki/https://github.com/Sineos/redmatic-flow-sysinfo/blob/master/README_DE.md)
* Sonstiges
  * [Dashboard Screenshots](https://github.com/hobbyquaker/RedMatic/wiki/Dashboard-Screenshots)


## Lizenzen

* [RedMatic](https://github.com/hobbyquaker/RedMatic) © 2018 Sebastian Raff and RedMatic Contributors, licensed under [Apache License 2.0](LICENSE)
* [RedMatic Documentation](https://github.com/hobbyquaker/RedMatic/wiki) © 2018 Sebastian Raff and RedMatic Contributors, licensed under [CC BY-SA License 4.0](https://creativecommons.org/licenses/by-sa/4.0/)
* [Third Party Licenses](LICENSES.md)

DIE SOFTWARE WIRD OHNE JEDE AUSDRÜCKLICHE ODER IMPLIZIERTE GARANTIE BEREITGESTELLT, EINSCHLIEẞLICH DER GARANTIE ZUR 
BENUTZUNG FÜR DEN VORGESEHENEN ODER EINEM BESTIMMTEN ZWECK SOWIE JEGLICHER RECHTSVERLETZUNG, JEDOCH NICHT DARAUF 
BESCHRÄNKT. IN KEINEM FALL SIND DIE AUTOREN ODER COPYRIGHTINHABER FÜR JEGLICHEN SCHADEN ODER SONSTIGE ANSPRÜCHE HAFTBAR
ZU MACHEN, OB INFOLGE DER ERFÜLLUNG EINES VERTRAGES, EINES DELIKTES ODER ANDERS IM ZUSAMMENHANG MIT DER SOFTWARE ODER 
SONSTIGER VERWENDUNG DER SOFTWARE ENTSTANDEN.
