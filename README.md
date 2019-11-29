# GVI Projekt 1 - Diagramme
author: Felix Schick (71scfe1bif), Nicolas Mohr (81moni1bif)  
date: 29. Movember 2019

## Aufgabe 1 - Bevölkerungsdichte in Europa

Der Datensatz, welcher für diese Aufgabe benutzt werden sollte bestand aus mehreren Sätzen des Dateiformats **Shapefile**. Dieses von ESRI entwickelte Dateiformat wird als Container für vektorielle Geodaten benutzt.

Es existiert eine JavaScript Library namens [shapefile.js](https://github.com/calvinmetcalf/shapefile-js), welche Funktionalitäten zum parsen von Shapefiles bietet.

Da sich das Shapefile Format aus verschiedenen Datein zusammensetzt, war der erste Schritt das zusammenführen der Datein durch komprimieren. Die für uns relevanten Daten befinden sich im *admin00* Shapefile. Dieser Datensatz beinhaltet die meisten Länder der Welt, Bundesländer und Regionen und Informationen zu Bevölkerung und Fläche jener.

![shapefiles](documentation/pics/admin_files.png)

Als nächster Schritt kann die komprimierte Shapefile eingelesen werden und als GeoJson genutzt werden. Die GeoJson ist nach Regionen sortiert, dies erlaubt uns für jede Region eine Bevölkerungsdichte zu berechnen und ihr eine Farbe zuzuweisen.
Diese Daten können wir dann über unseren Tiles Layer legen.

![europa](documentation/pics/europe_far.png)

Als letzten Schritt werden noch eine Legende und Pop-ups für die Regionen hinzugefügt um die genaue Bevölkerungsdichte dieser abzubilden. 

![pop-up](documentation/pics/europe_pup.png)

## Aufgabe 2 - Web-Karte mit Points of Interest 

## Aufgabe 3 - Karte Sustainable Indicators in Europa (5 Punkte) 
