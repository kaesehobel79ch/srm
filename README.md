# `SRM – System Resource Monitor`

SRM zeigt auf einen Blick, wie stark Ihr Rechner gerade arbeitet. Alles steht auf einer einzigen Oberfläche, es gibt nichts umzuschalten.

**[Herunterladen (neueste Version)](https://github.com/kaesehobel79ch/srm/releases/latest)**

Kostenlos (Freeware) von Käse_Hobel.

## Installieren

1. Unter „Herunterladen“ die Datei `SRM-<Version>.zip` laden.
2. ZIP entpacken.
3. `SRM-Setup.exe` starten und den Schritten folgen.

## Was angezeigt wird

- Auslastung von Prozessor und Grafikkarte
- Temperatur von Prozessor und Grafikkarte
- Arbeitsspeicher und Grafikspeicher
- Netzwerk, ankommend und abgehend
- Die sechs Programme mit dem höchsten Speicherverbrauch
- Die laufenden Verbindungen nach aussen, mit Namen statt nackten Adressen
- Prozessor und Grafikkarte im Klartext
- Die Kernspannung von Prozessor und Grafikkarte

Die Werte stehen auf Rundinstrumenten mit dreifarbiger Skala: grün, gelb, rot. Das Fenster lässt sich frei in der Grösse ändern, bis zum Vollbild. Helle und dunkle Darstellung richten sich nach der Einstellung von Windows.

## Verbindungen nach aussen

SRM zeigt, welche Programme gerade nach aussen verbunden sind und wohin. Bekannte Anbieter erscheinen mit Namen, Geräte im eigenen Netz sind als Heimnetz gekennzeichnet. Kommt eine Verbindung von ausserhalb des eigenen Netzes herein, erscheint eine deutliche Warnzeile.

SRM liest diese Angaben nur: es trennt nichts, blockiert nichts und verändert nichts am Netzwerk. Es ist weder eine Firewall noch ein Virenschutz und ersetzt beides nicht. Die Namen holt SRM beim Namensdienst, den der Rechner ohnehin benutzt; es wird kein fremder Dienst im Internet befragt.

## Grafik neu starten

Bleibt das Bild nach einem Spielabsturz schwarz oder flackert es, setzt ein Schalter den Grafiktreiber zurück. Vorher wird gefragt. Es wird nichts installiert und nichts an den Einstellungen geändert.

## Temperaturmessung und PawnIO

Die genaue Temperatur des Prozessors kann nur ein Programm mit einem Treiber im Systemkern auslesen. SRM verwendet dafür PawnIO, einen signierten Treiber, den Windows auch bei eingeschalteter Speicherintegrität nicht sperrt.

PawnIO liegt dem Setup bei. Beim Installieren werden Sie gefragt, ob es mitinstalliert werden soll. Ohne PawnIO läuft SRM genauso, nur mit der ungenaueren Temperatur aus dem BIOS. PawnIO stammt nicht von mir, wird als eigenes Programm eingetragen und lässt sich jederzeit wieder entfernen: [pawnio.eu](https://pawnio.eu)

## Voraussetzungen

- Windows 11 (64 Bit); Windows 10 ebenfalls, sofern das System auf dem letzten Stand ist
- Administratorrechte (nur zum Lesen der Sensoren; SRM verändert nichts am System)

Das Programm ist nicht digital signiert. Beim ersten Start kann sich deshalb der Windows-Schutz SmartScreen oder ein Virenscanner melden. Das ist ein Fehlalarm.

## Echtheit prüfen

Zu jedem Download gehören eine Prüfsumme (`.sha256`) und eine Unterschrift (`.asc`) mit dem Schlüssel von Käse_Hobel.

## Nutzungsbedingungen

Es gelten die [Nutzungsbedingungen](Nutzungsbedingungen.txt). Kurz: kostenlos nutzbar, Weitergabe nur unverändert und vollständig, nicht gegen Entgelt. Der Quellcode wird nicht veröffentlicht. Die Lizenzen der eingebauten fremden Bestandteile liegen nach der Installation im Programmordner.

Bei der Entwicklung wurde KI-Unterstützung eingesetzt.
