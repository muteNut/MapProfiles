## 6. Layout

Der Layout-Manager bietet zahlreiche Optionen, die hier kurz beschrieben werden. Ein so erstelltes Layout kann als Rastergrafik (zB `*.png`) oder PDF exportiert werden.

### 6.1 Layoutmanager & Page Properties

Zuerst ist es sinnvoll, die Seitendimensionen festzulegen. Sie orientieren sich an der gewünschten Abbildungsgröße im Bericht &ndash; bei einheitlichem Layout ist auch eine einheitliche Größe aller Karten naheliegend.

Dabei kann man sich an der Form der Untersuchungsregion und der Lesbarkeit orientieren. Für die Zentralregion OÖ habe ich zB eine Breite von 180mm gewählt, sodass die Karte eine volle Seitenbreite einnimmt. Daher erübrigen sich Textumfluss-Optionen. Alternativ wäre es denkbar, die Breite so zu wählen, dass zwei Karten nebeneinander auf eine A4-Seite passen. Das bietet sich bei einem Layout an, das in zwei Spalten struktiert ist: entweder man platziert die Karten paarweise nebeneinaner oder fügt sie einzeln an der passenden Stelle in die Textspalten ein. Möglicherweise ist die Untersuchungsregion aber so groß, dass die Karte dann nicht mehr lesbar wäre...

Wir erstellen zuerst ein neues Layout über `Insert` &ndash; `New Layout` &ndash; `Custom Page Size`. Hat man in der Eile auf eines der vorgefertigten Papierformate geklickt, kann man die Abmessungen auch nachträglich anpassen: in die `Page Properties` gelangt man über einen Rechtsklick in die leere Arbeitsfläche &ndash; `Properties` &ndash; `Page Setup`.

### 6.2 Map Elements

Eine Karte sollte stets ein paar Elemente aufweisen wie zum Beispiel:

#### 6.2.1 Legende
Das Legendenwerkzeug in ArcGIS kann etwas tricky sein. An dieser Stelle ist es am einfachsten, auf Erklärvideos zu verweisen:

[![Legends Tutorial in ArcGIS Pro](http://img.youtube.com/vi/kB_WSJZDzfk/0.jpg)](https://www.youtube.com/watch?v=kB_WSJZDzfk "Legends Tutorial in ArcGIS Pro")

Zu beachten ist, dass jeder einzelne Layer, der ein **Unterobjekt der Legende** ist, deaktiviert (=ausgeblendet) werden kann. Diese Sichtbarkeit gilt **nur** für die Legende, nicht für die Map!

#### 6.2.2 Massstab

Ein Massstab muss vorhanden sein und kann durch Klick auf `Scale Bar` eingefügt werden. Darstellungsstil und Optionen, wie zB die Teilungen usw. können individuell gewählt werden.

#### 6.2.3 Nordpfeil

Obwohl üblicherweise alle Karten per Default genordet sind, sollte ein Nordpfeil eingefügt werden. Je nach Projektion weist dieser Pfeil eine geringfügige Rotation auf, die angepasst bzw. korrigiert werden kann, indem der `Type` auf `Map North` gesetzt wird.

**Nicht notwendig, aber möglicherweise sinnvoll sind Elemente wie:**

#### 6.2.4 Textelemente, Formen

Ein Kartentitel ist üblicherweise ein Element, das auf keiner Karte fehlen sollte. Bei thematischen Karten für den Bericht kann diese Funktion vom Titel der Legende bzw. vom hauptsächlich abgebildeten Layer in der Legende übernommen werden. Flächen oder Linien, ... können die Karte optisch aufwerten. Ich mag semitransparente Overlays gerne, um bspw. Nordpfeil und Massstabsleiste leicht von der im Hintergrund liegenden Karte abzuheben.

#### 6.2.5 Overview Map

Zur Orientierung kann eine Übersichtskarte eingefügt werden. Dazu wird ein neuer Map Frame eingefügt und die passende Map gewählt. Während der neu erstellte Map Frame aktiv ist, kann ein `Extent Indicator` eingefügt werden. Damit wird der in `Map Frame` abgebildete Bereich in `Map Frame 1` hervorgehoben. Die Darstellungsparameter können je nach Bedarf angepasst werden. Dieses Element ist zB für die Übersichtskarte empfehlenswert, kann bei den nachfolgenden thematischen Karten aber weggelassen werden.

Eine detaillierte Beschreibung bietet dieses Video:

[![Extent Indicators in ArcGIS Pro ](http://img.youtube.com/vi/CHe-AANSLYM/0.jpg)](https://www.youtube.com/watch?v=CHe-AANSLYM "Extent Indicators in ArcGIS Pro")

### 6.3 Export

Zuletzt kann das erstellte Layout über `Share` &ndash; `Export Layout` exportiert werden. Je nachdem, mit welcher Software der Bericht erstellt wird, bietet sich ein PDF (zB bei Layout in InDesign) eher an. Dazu gibt es passende Presets (zB Vector PDF).

Bevorzugt man, den Bericht in Word oä zu verfassen, ist es wahrscheinlich sinnvoller, ein JPEG oder PNG zu exportieren. Der Dateityp kann nach Klick auf das Preset auch noch über `File Type` angepasst werden.

[Zurück](./join.md)

**Weiter mit: [Datenverwaltung: Tipps](./tips.md)**
