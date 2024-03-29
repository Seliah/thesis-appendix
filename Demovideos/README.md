# Demovideos

## Allgemeine Hinweise

Hier sind Videos dargestellt, die die im praktischen Projekt implementierten Funktionen veranschaulichen. Gleichzeitig werden hiermit korrespondierende Test-Cases protokolliert.
Zu jedem Video existiert eine kurze Beschreibung.

Die hier dargestellten Videos wurden komprimiert, um Speicherressourcen für die Abgabe dieser Arbeit zu schonen. Die wichtigen Elemente der Videos, die Markierungen von Erkennungen oder Konfigurationen und Logausgaben, sind jedoch trotzdem erkennbar. Es empfiehlt sich, die Videos im Vollbildmodus nachzuvollziehen.

## Bewegungssuche

https://github.com/Seliah/thesis-appendix/assets/52240180/98de66ae-1659-45d7-9327-7c5195587431

Alternativ siehe "bewegungssuche.mp4" im lokalen Verzeichnis.

Beschreibung: Zu Beginn ist zu sehen, wie eine Kamera ausgewählt wird und die Heatmap der Kamera eingeblendet wird. Anschließend ist zu sehen, wie ein bestimmter Bereich im Bild für die Bewegungssuche ausgewählt wird. Unten im Bild (in der Zeitleiste) erscheinen Markierungen, die Bewegungsereignisse im markierten Bereich repräsentieren. Wird ein Zeitpunkt für die Wiedergabe ausgewählt, wo keine Markierungen sind, ist keine Person im markierten Bereich zu sehen. Wird hingegen ein Punkt gewählt, wo Markierungen sind, ist der Autor im markierten Bereich zu sehen. Anschließend wird der ausgewählte Bildbereich noch verschoben und in der Größe verändert. Hier ist zu sehen, dass die Markierungen unten reagieren. Sind Bildbereiche ausgewählt, wo wenig Bewegung war, sind entsprechend weniger Markierungen zu sehen. Abschließend wird die Auswahl mit einem Rechtsklick aufgehoben und auch die Markierungen verschwinden.

## Regalüberwachung

https://github.com/Seliah/thesis-appendix/assets/52240180/7b84cdc9-6597-4816-a404-8b0ff8e268f0

Alternativ siehe "regalüberwachung.mp4" im lokalen Verzeichnis.

Spezifischer Hinweis: Die Framerate des Videos ist bewusst gering, weil die Anzahl der Analysen im Sinne der Performanceoptimierung minimiert worden ist.

Beschreibung: Im Video entnimmt der Autor sechs Mal Waren aus einem Regal, wobei vier Lücken entstehen. Ganz am Anfang des Videos ist bereits ganz rechts im Bild eine Lücke vorhanden. Als Reaktion darauf ist unten in der Konsole bereits eine Logausgabe „Neue Entnahme“ zu sehen. Als erstes entnimmt der Autor rechts im Bild Waren und eine neue Lücke entsteht. Auch hier entstehe eine Logausgabe „Neue Entnahme“. Anschließend verdeckt der Autor die Lücke bewusst mit seinem Körper. Es ist zu sehen, dass dies nicht dafür sorgt, dass „Neue Entnahme“ wiederholt ausgegeben wird. Die Verdeckung konnte als Problem also erfolgreich berücksichtigt werden. Auch fällt zu diesem Punkt bereits auf, dass manchmal Fehlerkennungen passieren. Diese lösen jedoch auch nicht die Erkennung einer Entnahme aus. Die Filterung von einzelnen Erkennungen funktioniert also auch. Anschließend wird links im Bild Ware in sehr schräger Perspektive entnommen. Dies wird auch korrekt erkannt. Als nächstes wird eine sehr schmale Lücke geöffnet. Dies wird nicht erkannt. Anschließend wird eine weitere schmale Lücke geöffnet, die jedoch erkannt wird. Diese wird zudem erweitert, was auch korrekt erkannt wird. Abschließend wird noch eine Entnahme ohne neue Lücke getätigt. Diese wird auch nicht erkannt.

## Integration externer Systeme

### Schlangenerkennung

https://github.com/Seliah/thesis-appendix/assets/52240180/7bd1a40e-6e47-4034-98ab-82e0ef781a63

Alternativ siehe "schlangenerkennung.mp4" im lokalen Verzeichnis.

Beschreibung: Das Video zeigt den Autor im Büro von Adeck Systems. Zu erkennen ist ein markierter Bereich im Bild, der jenen Bereich abdeckt, wo eine „Warteschlange“ zu erwarten ist. In einem realen Szenario wäre dies beispielsweise der Bereich vor Kassen, in diesem Test ist es ein willkürlicher Bereich. Der Autor betritt den konfigurierten Bereich im Bild und löst mit seinem fortlaufenden Aufenthalt darin die Erkennung einer Wartschlange aus. Dies ist durch den erscheinenden roten Hintergrund signalisiert. In der ebenfalls zu sehenden Konsole (oben) wird die Ausgabe des implementierten Programmes dargestellt. 

### Manipulationserkennung

https://github.com/Seliah/thesis-appendix/assets/52240180/8817eb31-a609-47d0-a7c3-0131c01d798f

Alternativ siehe "tampering.mp4" im lokalen Verzeichnis.

Beschreibung: Der Autor verdeckt das Videobild mit seiner Hand und simuliert somit eine Manipulation, die beispielsweise mit Spray-Farbe umgesetzt wurde. Nach einigen Sekunden wird eine Manipulationserkennung in der Konsole angezeigt.

### Linienüberwachung

https://github.com/Seliah/thesis-appendix/assets/52240180/b8bb1a39-040c-4c32-9d2c-53caf5ef5f48

Alternativ siehe "linienüberwachung.mp4" im lokalen Verzeichnis.

Beschreibung: Im Videobild ist eine Linie mit einer gelben Strecke markiert. Der grüne Bereich beschreibt den Bereich, in dem Erkennungen möglich sind (hier maximiert). Überschreitet der Autor die Linie von rechts nach links, wird eine Erkennung in der Konsole ausgegen. Überschreitet er sie von links nach rechts, geschieht dies nicht.

### Regionsmonitoring

https://github.com/Seliah/thesis-appendix/assets/52240180/3930bb88-2561-4643-ad85-8b05e5466881

Alternativ siehe "regionsmonitoring.mp4" im lokalen Verzeichnis.

Beschreibung: Im Videobild ist ein Bereich mit einem gelben Viereck markiert. Bewegt sich der Autor in diesen Bereich, wird eine Erkennung in der Konsole protokolliert. Verlässt er ihn, wird dies ebenfalls protokolliert.
