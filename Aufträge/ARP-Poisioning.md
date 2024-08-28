# Arp Poisioning

## Was ist ARP Poisioning 
ARP Poisoning, auch bekannt als ARP-Spoofing oder ARP Cache Poisoning, ist eine Form von Man-in-the-Middle-Angriff (MitM), bei dem ein Angreifer die Address Resolution Protocol (ARP)-Tabellen in einem Netzwerk manipuliert, um den Datenverkehr zwischen Geräten abzufangen, umzuleiten oder zu manipulieren.

### So funktionier ARP Poisioning
![image](https://github.com/user-attachments/assets/befd3266-71b3-4de4-8e3a-70629d5f3f23)
Der Angreiffer sendet gefälschte ARP-Antworten ins Netzwerk.Diese falschen Nachrichten weisen den Geräten im Netzwerk eine falsche MAC-Adresse für eine bestimmte IP-Adresse zu, beispielsweise die des Routers oder eines anderen Geräts.

### Das ist das gefährliche an diesem Angriff 
Aufgrund der manipulierten ARP-Tabellen senden die betroffenen Geräte ihre Datenpakete an die MAC-Adresse des Angreifers, anstatt an den legitimen Empfänger.
Und so kann der Angreifer nun die Daten abfangen, analysieren, manipulieren oder an den eigentlichen Empfänger weiterleiten, wodurch ein Man-in-the-Middle-Angriff entsteht.
