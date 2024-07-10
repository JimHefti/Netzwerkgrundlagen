# Kollisionsdomäne (CSMA/CD)
## wie viel Kolisions Domänen hat es bei einem hub 
Ein Hub arbeitet auf der OSI-Schicht 1 und leitet alle eingehenden Datenpakete an alle anderen Ports weiter. Daher gibt es bei einem Hub nur eine Kollisionsdomäne. Das bedeutet, dass alle Geräte, die an den Hub angeschlossen sind, sich die Bandbreite teilen und miteinander konkurrieren, was zu Kollisionen führen kann, wenn mehrere Geräte gleichzeitig senden.

## Wie viele Kolisions Domänen bei einem Hub
Ein Switch arbeitet auf der OSI-Schicht 2 und leitet Datenpakete gezielt anhand der MAC-Adressen der angeschlossenen Geräte weiter. Jeder Port eines Switches bildet dabei eine eigene Kollisionsdomäne. Dies reduziert die Anzahl der Kollisionen erheblich, da jedes Gerät eine direkte Verbindung zum Switch hat und nicht mit anderen Geräten um die Bandbreite konkurrieren muss.
