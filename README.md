ffrlbeipackzettel
=================
Ein Beipackzettel für Freifunkrouter, erstellt mit TeX Live incl. pgf/TikZ.

Anpassen
========
tex-Datei für eigene Community anpassen, dann übersetzen mit pdflatex Beipackzettel_Community.tex

Quellcodeaufbau
===============
Um eine Dreiteilung einer A4-Seite zu erhalten, wird die Klasse leaflet verwendet.
leaflet erstellt eine dreigeteilte A4-Seite und beginnt mit dem Druck in der rechten Spalte der ersten Seite, 
dann werden die drei Spalten der Rückseite bedruckt, die auf dem Kopf stehen und der Reihe nach gefüllt werden,
bis die letzten beiden Spalten der ersten Seite wieder drankommen.

Hier wird nun gesagt, dass nur die Rückseite erstellt werden soll, außerdem nicht auf dem Kopf stehend.
Der zu druckende Inhalt wird einmal als Kommando \inhalt definiert, dann zigmal wiederholt abgedruckt:
Das erste mal, um die rechte Spalte der ersten Seite zu füllen (ist in der pdf dann nicht zu sehen) 
und dann für jede Spalte der Rückseite ein weiteres mal, so dass drei identische Spalten auf einem A4-Blatt 
entstehen, das dann zerschnitten werden kann.
Eine Falzmarkierung ist noch zu sehen, die kann bei Bedarf entfernt werden, siehe leaflet-manual:
http://www.ctan.org/tex-archive/macros/latex/contrib/leaflet

Das Logo wurde von der SVG-Datei des offiziellen Freifunklogos nach TikZ portiert und wird skaliert.
Die Dicke des dicken Außenkreises ist im Verhältnis normalerweise dicker (6mm statt 4mm), aber dann sieht
das Logo nach der Skalierung nicht mehr gut aus.