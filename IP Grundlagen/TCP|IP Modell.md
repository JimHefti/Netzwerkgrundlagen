# TCP/IP Modell
![image](https://github.com/JimHefti/Netzwerkgrundlagen/assets/160615771/adfb3700-3261-42d1-a60c-bc3523aafaaa)

## Anwendungsschicht: 
Diese Schicht umfasst Protokolle, die für Endnutzeranwendungen wie E-Mail, Webbrowser und Dateiübertragungen verwendet werden.
## Transportschicht: 
Sie ist zuständig für die Übertragung von Daten zwischen Endsystemen und bietet Dienste wie die Fehlerkorrektur und Flusskontrolle an.
## Internetschicht: 
Diese Schicht kümmert sich um die Weiterleitung von Paketen über Netzwerkgrenzen hinweg und verwendet dafür das Internetprotokoll (IP).
## Netzwerkzugangsschicht: 
Sie bezieht sich auf physikalische und hardwarenahe Protokolle, die für die tatsächliche Übertragung der Daten über das Medium verantwortlich sind.


# Protokolle

## Schicht 1 (Netzwerkzugangsschicht)
ICMP: Wird für Fehlermeldungen und Diagnosezwecke verwendet, z.B. bei der Durchführung von Ping-Tests.

ARP: Übersetzt IP-Adressen in MAC-Adressen

RARP: Übersetzt MAC-Adressen in IP-Adressen

## Schicht 2 (Internetschicht)
TCP: Bietet eine zuverlässige, verbindungsorientierte Kommunikation zwischen Anwendungen.

UDP: Bietet eine verbindungslose Kommunikation, die schneller, aber weniger zuverlässig ist als TCP.

## Schicht 3 (Transportschicht)
ICMP,ARP und RARP


## Schicht 4 (Anwendungsschicht)
HTTP: Wird zum Übertragen von Webseiten über das Internet verwendet.

HTTPS: Eine sichere Version von HTTP, die Verschlüsselung über TLS/SSL verwendet.
