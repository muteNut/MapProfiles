## 3. Vektoroperationen

Ein kurzer Überblick über die in diesem Kurs wichtigsten Vektoroperationen. Sämtliche Tools können direkt über die Suchleiste geöffnet werden oder über den Ribbon **Analysis** &ndash; **Tools**.

### 3.1 Pairwise Clip

Clip entfernt alles, außer den Inhalten, die sich innerhalb des Clip Features befinden. Die Attribute des Clip Features werden nicht berücksichtigt.

[![Link zu ArcGIS Hilfe](https://pro.arcgis.com/en/pro-app/latest/tool-reference/analysis/GUID-6D3322A8-57EA-4D24-9FFE-2A9E7C6B29EC-web.png)](https://pro.arcgis.com/en/pro-app/latest/tool-reference/analysis/pairwise-clip.htm)

Wir können den Pairwise Clip beispielsweise verwenden, um Einrichtungen, die sich außerhalb der Region befinden, schnell zu entfernen. In diesem Beispiel könnte der Punkt-Layer mit Einrichtungen das *Input Feature* sein, die Region das *Clip Feature*. In *Output Feature Class* kann der gewünschte Speicherort des Outputs festgelegt werden.

### 3.2 Pairwise Intersect

Das Ergebnis des Intersects sind alle sich überlagernden Features. Inhalte, die keine Überlagerung vorweisen, werden verworfen. Anders als beim Clip werden sämtliche Attribute aller Input Features übernommen. Wird beispielsweise ein Polygon-Layer mit *Stehenden Gewässern* mit einem Polygon-Layer *Gemeindegrenzen* verschnitten, so wird der Output je Wasserfläche anhand der Gemeindegrenzen neu unterteilt, es entstehen also neue Features.

[![Link zu ArcGIS Hilfe](https://pro.arcgis.com/en/pro-app/latest/tool-reference/analysis/GUID-93B78EC9-4024-43AC-87BF-765FAD873B00-web.gif)](https://pro.arcgis.com/en/pro-app/latest/tool-reference/analysis/pairwise-intersect.htm)

Wir können den Pairwise Intersect beispielsweise verwenden, um den Einrichtungen innerhalb der Region Informationen zuzuweisen, in welcher Gemeinde sie sich befinden. Dabei sind Einrichtungen und Gemeinden die *Input Features*.

### 3.3 Pairwise Dissolve

Dissolve fügt einzelne Features zu einem Teil zusammen. Die Auflösung kann dabei anhand einer Spalte erfolgen.

[![Link zu ArcGIS Hilfe](https://pro.arcgis.com/en/pro-app/latest/tool-reference/analysis/GUID-B1553328-7E02-4A67-ABC9-2391F5D6C2CC-web.png)](https://pro.arcgis.com/en/pro-app/latest/tool-reference/analysis/pairwise-dissolve.htm)

Wir können den Pairwise Dissolve dazu benutzen, um Gemeinden zu Bezirken oder Bundesländern zusammenzufassen, sofern diese Information in der Attributtabelle vorhanden ist. In diesem Fall sind die Gemeinden das *Input Feature*, das *Dissolve Field* die Spalte mit der Bundesland-Information. Bleibt das *Dissolve Field* leer, werden sämtliche Features vereint.

[Zurück](./add_content.md)

**Weiter mit: [Attribute Table](./attr.md)**
