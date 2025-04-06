# Map Sources
JSON files for ArcGIS vector tiles
erstellt mit [Vector Tile Style Editor](https://developers.arcgis.com/vector-tile-style-editor/).

* [Unlabeled topgraphical map](https://raw.githubusercontent.com/muteNut/MapProfiles/refs/heads/main/res/WorldTopo_Unabeled.json)
* DTM OOe 10m median cells merged (src: BEV) [download here](http://nc.dazzr.space/DTM_OOe.zip)
> Grundlage ist das [ALS DTM](https://data.bev.gv.at/geonetwork/srv/ger/catalog.search#/search?isTemplate=n&resourceTemporalDateRange=%7B%22range%22:%7B%22resourceTemporalDateRange%22:%7B%22gte%22:null,%22lte%22:null,%22relation%22:%22intersects%22%7D%7D%7D&sortBy=creationDateForResource&sortOrder=desc&from=1&to=100&any=ALS%20DTM%20H%C3%B6henraster%201m) vom BEV, die Kacheln wurden kombiniert und vergröbert (focal statistics). Aufgrund des hohen Ressourcenbedarfs weist die Map an den Kanten Artefakte auf, was für den aktuellen Anwendungszweck vernachlässigbar ist.

# Andere Kartendaten
* [Verwaltungsgrenzen 1:250 000](https://www.data.gv.at/katalog/de/dataset/vgd-stichtagsdaten-1-250-000) für Übersichtskarte evtl.
* [Gemeindeschwerpunkte](https://data.statistik.gv.at/web/meta.jsp?dataset=OGDEXT_GEM_MP_1)
* [Regionale Gliederung in Bezirke](https://www.data.gv.at/katalog/de/dataset/stat_gliederung-osterreichs-in-politische-bezirke131e2)
* [Stehende Gewässer](https://www.data.gv.at/katalog/de/dataset/gesamtgewssernetzstehendegewsser)
* [Fließende Gewässer](https://www.data.gv.at/katalog/de/dataset/gesamtgewssernetzfliessgewsserrouten)
* [Straßen](strassen.geojson)
