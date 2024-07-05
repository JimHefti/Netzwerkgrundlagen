# ISO/OSI Referenzmodell
![image](https://github.com/JimHefti/Netzwerkgrundlagen/assets/160615771/bc6c7586-d302-4f13-a90a-011f66da0d52)

## Definition
Das Open Systems Interconnection (OSI)-Modell ist ein Grundstruktur, das festlegt, wie Netzwerke miteinander kommunizieren und Daten von einem Sender zu einem Empfänger senden.Das Modell wird dazu genutzt, jede Komponente in der Datenkommunikation genau zu beschreiben, sodass Regeln und Standards definiert werden können, wie Anwendungen und Netzwerkinfrastruktur aussehen sollten.
Das OSI-Modell enthält sieben Schichten, die konzeptionell von unten nach oben aufeinander „gestapelt“ sind. Die OSI-Modell-Schichten bestehen aus: Bitübertragung, Sicherung, Vermittlung, Transport, Sitzung, Darstellung und Anwendung.


## 7. Schicht – Anwendungsschicht
Die siebte Schicht kennen die meisten Menschen, weil sie direkt mit dem Nutzer kommuniziert. Eine Anwendung, die auf einem Gerät läuft, mag vielleicht mit anderen OSI-Schichten kommunizieren; die Benutzeroberfläche jedoch läuft auf der siebten Schicht. Ein E-Mail-Client, der Nachrichten zwischen einem Anwender und einem Server überträgt, befindet sich beispielsweise auf der siebten Schicht. Wenn eine Nachricht in der Client-Software ankommt, ist es die Anwendungsschicht, die sie dem Nutzer anzeigt. Anwendungsprotokolle für diese Schicht sind etwa SMTP (Simple Mail Transfer Protokoll) und HTTP, das Protokoll für die Kommunikation zwischen Browsern und Webservern.
![image](https://github.com/JimHefti/Netzwerkgrundlagen/assets/160615771/436737d6-5f2b-4dde-b122-4fdd6c1281c8)


## 6. Schicht – Darstellungsschicht
Die Anwendungsschicht zeigt dem Nutzer Informationen, aber die Darstellungsschicht des OSI-Modells bereitet die Daten so auf, dass sie dem Nutzer überhaupt erst angezeigt werden können. Es ist üblich, dass zwei verschiedene Anwendungen die gleiche Kodierung verwenden. Die Kommunikation mit einem Webserver über HTTPS nutzt zum Beispiel verschlüsselte Informationen.
Die Darstellungsschicht ist dabei für das Ver- und Entschlüsseln der Informationen verantwortlich, sodass sie dem Nutzer in einfacher Textform angezeigt werden können. Die Darstellungsschicht übernimmt außerdem die Komprimierung und Dekomprimierung von Daten, während sie von einem Gerät zum nächsten wandern.
![image](https://github.com/JimHefti/Netzwerkgrundlagen/assets/160615771/c0d568c6-be5e-435d-bfed-1589337e184c)


## 5. Schicht – Sitzungsschicht
Um zwischen zwei Geräten zu kommunizieren, muss eine Anwendung zuerst eine Sitzung (Session) herstellen. Eine Sitzung ist für jeden Nutzer einzigartig und identifiziert ihn eindeutig auf dem Remote-Server. Die Session muss so lange offen bleiben, wie Daten übertragen werden, aber danach muss sie sich schließen. Wenn große Volumen an Daten übertragen werden, ist es die Aufgabe der Sitzung, den erfolgreichen Tranfer der Daten sicherzustellen und eine erneute Übertragung einzuleiten, sollten die Daten unvollständig sein. Wenn zum Beispiel 10MB Daten übertragen werden und nur 5 MB ankommen, sorgt die Sitzungsschicht dafür, dass nur die fehlenden 5 MB erneut übertragen werden. Diese Art des Transfers macht die Kommunikation in einem Netzwerk effizienter, statt Ressourcen auf das erneute Übertragen der gesamten Datei zu verschwenden.

## 4. Schicht – Transportschicht
Die Transportschicht ist dafür zuständig, Daten in kleinere Einheiten zu zerlegen. Wenn Daten innerhalb eines Netzwerks übertragen werden, werden sie nicht als ein Gesamtpaket versendet. Um die Übertragung effizienter und schneller zu machen, bricht die Transportschicht die Daten stattdessen in kleinere Bestandteile auf. Diese kleineren Teile enthalten Header-Informationen, sodass sie am Zielgerät wieder zusammengesetzt werden können. Segmentierte Daten besitzen außerdem eine Fehlerkontrolle, um der Sitzungsschicht mitzuteilen, ob sie eine erneute Verbindung herstellen muss, falls einzelne Packets fallen gelassen wurden oder unvollständig am Zielempfänger angekommen sind.
![image](https://github.com/JimHefti/Netzwerkgrundlagen/assets/160615771/28f4db36-0843-439d-bc41-58a88407df04)



## 3. Schicht – Vermittlungsschicht
Die Vermittlungsschicht zerlegt Daten auf dem Sendergerät in kleinere Einheiten und setzt sie auf dem Empfängergerät wieder zusammen, wenn die Übertragung zwischen zwei verschiedenen Netzwerken stattfindet. Bei der Kommunikation innerhalb eines Netzwerks ist die Vermittlungsschicht überflüssig, aber die meisten Nutzer verbinden sich mit mehreren Netzwerken, etwa mit einer Cloud. In dem Fall bewegen sich Daten zwischen verschiedenen Netzwerken, und dann übernimmt die Vermittlungsschicht die Aufgabe, kleine Daten-Packets zu erstellen, die zu ihrem Ziel geroutet und auf dem Empfängergerät dann erneut zusammengesetzt werden können.
![image](https://github.com/JimHefti/Netzwerkgrundlagen/assets/160615771/1db51879-e871-4451-9d4e-3ffecade9600)



## 2. Schicht – Sicherungsschicht
Während die Vermittlungsschicht die Kommunikation zwischen verschiedenen Netzwerken ermöglicht, überträgt die Sicherungsschicht Daten innerhalb des gleichen Netzwerks. Die Sicherungsschicht wandelt Packets, die sie von der Vermittlungsschicht erhält, in Blöcke (Frames) um. Genauso wie die Vermittlungsschicht führt die Sicherungsschicht eine Fehlerkontrolle und weitere Arbeitsprozesse durch, um eine erfolgreiche Übertragung zu gewährleisten.
![image](https://github.com/JimHefti/Netzwerkgrundlagen/assets/160615771/3fa2ca82-ca96-45fd-aab4-e86adf5cf85e)


## 1. Schicht – Bitübertragungsschicht
Wie der Name schon sagt, ist die Bitübertragungsschicht für das physische Gerät und die Komponenten zuständig, auf denen der Datentransfer abläuft, wie etwa Kabel und Router, die im Netzwerk installiert sind. Bei dieser Schicht sind Standards unerlässlich. Ohne Standards wäre eine Übetragung zwischen Geräten verschiedener Hersteller unmöglich.
![image](https://github.com/JimHefti/Netzwerkgrundlagen/assets/160615771/6b6d7fa7-5248-400b-b1c1-bc9c92ba8469)

