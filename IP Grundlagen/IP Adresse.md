# IP Adresse
![image](https://github.com/JimHefti/Netzwerkgrundlagen/assets/160615771/26695b59-dd25-46c3-b691-3ffacae1959f)

## Was ist eine IP Adresse
Eine IP-Adresse (Internet Protocol-Adresse) besteht aus (32bits/128bits) einer Abfolge von Zahlen, die jedem Gerät zugewiesen wird, das mit einem Computernetzwerk oder dem Internet verbunden ist.
Mithilfe von IP-Adressen werden Milliarden von Online-Geräten, wie Computer oder Mobiltelefone, identifiziert und unterschieden.

![image](https://github.com/JimHefti/Netzwerkgrundlagen/assets/160615771/8097b6af-6753-4ba5-9c80-7df8eaddf7aa)

## Arten 
statische IP-Adresse/dynamischen IP-Adresse

Es werden grundsätzlich zwei verschiedene Arten von IP-Adressen unterschieden. Die statische IP-Adresse sowie die dynamische IP-Adresse. Von einer statischen IP spricht man, wenn diese fest vergeben ist. Werden einem Computer während der Verbindung zum Internet wechselnde IP-Adressen zugewiesen, ist von der dynamischen IP-Adresse die Rede.
Statische IP-Adressen werden hingegen meist von Unternehmen genutzt, um innerhalb des Unternehmensnetzes zum Beispiel Zugriffe auf eine IP-Adresse besser steuern zu können.

## IPv4
IP-Adresse mit einem Bitcode von 32 Stellen oder auch vier Byte vor. Die IPv4 kann wahlweise als hexadezimale oder dezimale Zahlenkombination dargestellt werden. Für IPv4-Adressen wird üblicherweise die Dezimalschreibweise verwendet. Dazu werden die 32 Bit der IPv4-Adresse in jeweils 8 Bit aufgeteilt und durch Punkte getrennt.

![image](https://github.com/JimHefti/Netzwerkgrundlagen/assets/160615771/b6e5fe0a-7542-4a05-ac7d-42700debbb63)

## IPv6
Die IPv6 128-Bit-Adressen. Die Adresse wird hexadezimal in 16-Bit-Gruppen notiert. Hier stehen die letzten 64 Bit für die Host-Adresse. Eine gültige IPv6-Adresse wäre zum Beispiel:

1234:5678:90BC:DEFG:0000:0000:0000:2345

## IP Range
Bestimmt wird die Größe der Range durch die Subnetzmaske.
Der Beginn der IP-Range wird durch die eigentliche Netzwerkadresse begrenzt. Das Ende der IP-Range bildet die Broadcast-Adresse, die für alle mit dem gleichen Netzwerk verbundenen Geräte verwendet werden kann.

### Beispiel zu IP-Range
Die IP-Adresse lautet 192.168.10.1

Bei einer Standard-Subnetzmaske sind demzufolge weitere IP-Adressen innerhalb der Range bis 192.168.10.254 zu vergeben.

Je größer folglich die IP-Range ist, desto mehr Geräte können innerhalb eines Netzwerkes genutzt werden.


## Wichtig
- Eine Netzwerkadresse darf für jedes Geräte in einem Netzwerk nur einaml vergeben werden.
- Jedes Gerät hat seine eigene IP-Adresse
