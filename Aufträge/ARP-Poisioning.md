# Arp Poisioning

## Was ist ARP Poisioning 
ARP Poisoning, auch bekannt als ARP-Spoofing oder ARP Cache Poisoning, ist eine Form von Man-in-the-Middle-Angriff (MitM), bei dem ein Angreifer die Address Resolution Protocol (ARP)-Tabellen in einem Netzwerk manipuliert, um den Datenverkehr zwischen Geräten abzufangen, umzuleiten oder zu manipulieren.

### So funktionier ARP Poisioning
![image](https://github.com/user-attachments/assets/befd3266-71b3-4de4-8e3a-70629d5f3f23)

Der Angreiffer sendet gefälschte ARP-Antworten ins Netzwerk.Diese falschen Nachrichten weisen den Geräten im Netzwerk eine falsche MAC-Adresse für eine bestimmte IP-Adresse zu, beispielsweise die des Routers oder eines anderen Geräts.

### Das ist das gefährliche an diesem Angriff 
Aufgrund der manipulierten ARP-Tabellen senden die betroffenen Geräte ihre Datenpakete an die MAC-Adresse des Angreifers, anstatt an den legitimen Empfänger.
Und so kann der Angreifer nun die Daten abfangen, analysieren, manipulieren oder an den eigentlichen Empfänger weiterleiten, wodurch ein Man-in-the-Middle-Angriff entsteht.

## Wie nennt sich diese Attacke auch noch?
Diese Attacke wird auch ARP-Spoofing oder ARP Cache Poisoning genannt.




## Was ist das Ziel dieser Attacke?
Das Ziel von ARP Poisoning ist es, den Netzwerkverkehr umzuleiten, abzufangen oder zu manipulieren, indem gefälschte ARP-Nachrichten gesendet werden. Dadurch kann ein Angreifer sensible Informationen stehlen, Daten verändern oder den Netzwerkverkehr stören.




## Wer setzt diese Attacke ein?
Diese Attacke wird typischerweise von Cyberkriminellen, Hacker-Gruppen, oder Penetrationstestern eingesetzt. Cyberkriminelle nutzen sie für Datendiebstahl oder Spionage, während Penetrationstester sie verwenden, um Schwachstellen in Netzwerken aufzudecken.


## Was sind die Folgen dieser Attacke?

Datenverlust: Abfangen von vertraulichen Informationen wie Passwörtern oder Kreditkartendaten.

Datenmanipulation: Veränderung des Inhalts von Datenpaketen, was zu fehlerhaften oder falschen Informationen führen kann.

Netzwerkstörungen: Durch das Umleiten oder Blockieren von Daten kann der Netzwerkverkehr gestört oder lahmgelegt werden.

Vertrauensverlust: Bei wiederholten Angriffen kann das Vertrauen in die Netzwerk- und IT-Sicherheit stark beschädigt werden.


## Wie gefährlich sind solche Attacken?
ARP Poisoning ist sehr gefährlich, besonders in ungeschützten Netzwerken. Es ermöglicht Angreifern, unbemerkt Daten zu stehlen oder zu manipulieren, was zu erheblichen finanziellen und sicherheitstechnischen Schäden führen kann.


## Wie kann ein Unternehmen sich gegen diese Attacke schützen? (Aktiv, paasiv, mögliche Tools)
ARP-Überwachung: Setze Tools ein, die das Netzwerk kontinuierlich auf verdächtige ARP-Aktivitäten überwachen.
Statische ARP-Einträge: Lege für kritische Geräte im Netzwerk statische ARP-Einträge fest, die nicht manipuliert werden können.
VLANs: Segmentiere das Netzwerk, um die Ausbreitung eines Angriffs zu erschweren.
