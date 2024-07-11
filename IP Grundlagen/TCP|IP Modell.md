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




# Schicht 1 (Netzwerkzugangsschicht)
## Adressierung
### IP-Adressen
#### Aufbau
IPv4-Adressen bestehen aus 32 Bit und werden in vier Dezimalzahlen (je 8 Bit) dargestellt, getrennt durch Punkte (z.B., 192.168.1.1). IPv6-Adressen bestehen aus 128 Bit und werden in acht Gruppen von vier hexadezimalen Zahlen dargestellt, getrennt durch Doppelpunkte (z.B., 2001:0db8:85a3:0000:0000:8a2e:0370:7334).

#### Funktionalität
Identifizieren eindeutige Hosts und Netzwerkschnittstellen im Netzwerk.

#### Verwendung
Ermöglichen das Routing von Datenpaketen zwischen Netzwerken. Jede IP-Adresse ist einzigartig innerhalb eines Netzwerks und erlaubt die Zustellung von Datenpaketen an den richtigen Host.

## Protokolle
ICMP: Wird für Fehlermeldungen und Diagnosezwecke verwendet, z.B. bei der Durchführung von Ping-Tests.

ARP: Übersetzt IP-Adressen in MAC-Adressen

RARP: Übersetzt MAC-Adressen in IP-Adressen

# Schicht 2 (Internetschicht)
## Adressierung
### Portnummern

#### Aufbau
Portnummern sind 16-Bit-Zahlen, die spezifische Anwendungen oder Prozesse auf einem Host identifizieren. Es gibt 65.536 mögliche Portnummern, von denen die ersten 1.024 als "well-known ports" für häufig verwendete Protokolle reserviert sind (z.B., HTTP auf Port 80, HTTPS auf Port 443).

#### Funktionalität
Erlauben die Adressierung von spezifischen Diensten oder Anwendungen auf einem Host.

#### Verwendung
Bestimmen, welche Anwendung oder welcher Prozess die empfangenen Daten erhält. Z.B., ein Webserver auf einem Host könnte HTTP-Anfragen auf Port 80 empfangen.

## Protokolle
TCP: Bietet eine zuverlässige, verbindungsorientierte Kommunikation zwischen Anwendungen.

UDP: Bietet eine verbindungslose Kommunikation, die schneller, aber weniger zuverlässig ist als TCP.

# Schicht 3 (Transportschicht)
## Adressierung
### IP-Adressen
#### Aufbau und Funktionalität
Siehe Netzwerkschicht. Diese Adressen werden auch hier verwendet, da diese Schicht für das Routing von Paketen verantwortlich ist.
## Protokolle
ICMP,ARP und RARP


# Schicht 4 (Anwendungsschicht)
## Adressierung
### Domainnamen (DNS - Domain Name System)
#### Aufbau
Domainnamen sind hierarchische Namen, die durch Punkte getrennt sind (z.B., www.example.com). Sie bestehen aus mehreren Ebenen, wobei die höchste Ebene (Top-Level-Domain, z.B. .com) am Ende steht.
#### Funktionalität
Bieten menschenlesbare Adressen für IP-Adressen.
#### Verwendung
Werden vom DNS aufgelöst, um die IP-Adresse zu finden, die einer Domain entspricht. Erlauben Benutzern den einfachen Zugriff auf Webseiten und Dienste, ohne sich IP-Adressen merken zu müssen.

## Protokolle
HTTP: Wird zum Übertragen von Webseiten über das Internet verwendet.

HTTPS: Eine sichere Version von HTTP, die Verschlüsselung über TLS/SSL verwendet.

FTP: Dient dem Transfer von Dateien zwischen einem Client und einem Server.

SMTP: Wird zum Senden von E-Mails verwendet.

POP3: Werden zum Abrufen von E-Mails verwendet.

DNS: Übersetzt Domainnamen in IP-Adressen.

Telnet: Ermöglicht die Verbindung zu einem entfernten Rechner zur Verwaltung und Steuerung.

SSH: Eine sichere Alternative zu Telnet für die Verwaltung und Steuerung von entfernten Rechnern.





