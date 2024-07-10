# Broadcast-Domäne

# Beispiel einer Broadcast-Domain

## Netzwerkszenario

Stellen Sie sich ein kleines Büro-Netzwerk mit den folgenden Komponenten vor:

### Komponenten

1. **Switch A**
   - Verbunden mit:
     - PC1 (IP: 192.168.1.2)
     - PC2 (IP: 192.168.1.3)
     - PC3 (IP: 192.168.1.4)

2. **Router B**
   - Verbunden mit Switch A

3. **Switch C**
   - Verbunden mit:
     - PC4 (IP: 192.168.2.2)
     - PC5 (IP: 192.168.2.3)
     - PC6 (IP: 192.168.2.4)
   - Verbunden mit Router B

## Erklärung der Broadcast-Domänen

### Broadcast-Domain 1

- **Geräte:** PC1, PC2, PC3 und der mit Switch A verbundene Port des Routers B.
- **IP-Bereich:** 192.168.1.0/24
- **Verhalten:** Wenn PC1 ein Broadcast-Paket (z. B. eine ARP-Anfrage: "Wer hat die IP 192.168.1.3?") sendet, wird dieses Paket an PC2, PC3 und den Router gesendet. Alle Geräte in dieser Broadcast-Domain empfangen das Paket.

### Broadcast-Domain 2

- **Geräte:** PC4, PC5, PC6 und der mit Switch C verbundene Port des Routers B.
- **IP-Bereich:** 192.168.2.0/24
- **Verhalten:** Wenn PC4 ein Broadcast-Paket sendet, wird dieses Paket an PC5, PC6 und den Router gesendet. Alle Geräte in dieser Broadcast-Domain empfangen das Paket.

## Wichtige Punkte

- **Router als Broadcast-Domain-Grenze:**
  - Router fungieren als Grenze zwischen Broadcast-Domänen. Broadcast-Pakete werden nicht von einer Broadcast-Domain in eine andere weitergeleitet.
  - In unserem Beispiel verbindet der Router die beiden Broadcast-Domänen, leitet aber keine Broadcast-Pakete zwischen ihnen weiter.

- **Switches innerhalb einer Broadcast-Domain:**
  - Alle Geräte, die an denselben Switch oder an miteinander verbundene Switches (ohne Router dazwischen) angeschlossen sind, gehören zur gleichen Broadcast-Domain
