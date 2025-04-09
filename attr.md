## 4. Attribute Table

Eine wichtige Eigenschaft von Geodaten ist die Verknüpfung von Geometrie und Information. So kann jedes *Feature* in einem Layer unterschiedliche Attribute aufweisen. Die Tabelle kann durch Rechtsklick auf den entsprechenden Layer im `Table of Contents` &ndash; `Attribute Table` aufgerufen werden.

### 4.1 Datentypen

Jede Spalte weist einen Datentyp auf, der aufscheint, wenn man mit der Maus auf einem Spaltentitel bleibt.

<img src ="./img/type.jpg" alt="Screenshot von Datenspalte" width="500">

Alternativ lässt sich der Datentyp über `Table` &ndash; `Fields` nachprüfen. Dieser Typ ist bspw. wichtig, wenn zwei Tabellen miteinander [verknüpft](./join.md) werden sollen. Die für uns wichtigsten Datentypen sind in der Tabelle angeführt:

| Name | Eigenschaft |
| - | - |
| Text | reguläre alphanumerische Zeichenkette |
| Float | Gleitkommazahl, für die meisten Anwendungsfälle ausreichend |
| Double | Gleitkommazahl |
| Short | Ganzzahl zwischen -32 768 und 32 767 |
| Long | Ganzzahl zw. rund -2 und +2 Millionen |

**Allen numerischen Typen ist gemein, dass sie keine führende 0 unterstützen!**

### 4.2 Calculate

Mit dem Rechner können Attributwerte berechnet und ggf. neue Felder angelegt werden. Die Inhalte der bestehende Felder können so auch überschrieben bzw. aktualisiert werden. Sollte z.B. eine Spalte nicht dem gewünschten Datentyp entsprechen, legt man am einfachsten mit *Calculate* ein neues Feld an und füllt die Werte der bisherigen Spalte dort ein:

<img src="./img/calc1.jpg" alt="Screenshot von Calculate zum Erstellen einer neuen Spalte" width="500">

Der Calculator versteht auch Python. So kann zB Teil einer `Text`-Spalte extrahiert werden:

<img src="./img/calc2.jpg" alt="Screenshot von Calculate zum Extrahieren eines Strings" width="500">

Zudem können Funktionen definiert werden. Für diesen Kurs ist das aber irrelevant.

### 4.3 Filtern (Definition Query)

Die Features in einem Layer können anhand verschiedener Kriterien gefiltert werden. Das geschieht mit einer *Definition Query*, die über einen Doppelklick auf den entsprechenden Layer im `Table of Contents` auffindbar ist:

<img src="./img/dq1.jpg" alt="Screenshot von Definition Query" width="500">

Mit Klick auf `New definition query` kann ein neuer Filter erstellt werden:

<img src="./img/dq2.jpg" alt="Screenshot von Definition Query" width="500">

Ein ähnliches Ergebnis kann erzielt werden, wenn die Features eines Layers exportiert werden (`Rechtsklick auf Layer` &ndash; `Export Features`). Hier können Parameter gewählt werden, welche Features in einen neuen Layer exportiert werden sollen:

<img src="./img/export_features.jpg" alt="Screenshot von Export Features" width=500>

[Zurück](./vector.md)

**Weiter mit: [Daten verknüpfen (Joins)](join.md)**
