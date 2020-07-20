# Image Classification


### Projektbeschreibung

Bei diesem Projekt geht es darum mit dem Datensatz "Fruits-360" (bei Kaggle zu finden) den Einfluss von Hyperparametern auf ein Model darzustellen.
Dafür wurde als Lösungsansatz "Transfer Learning" ausgewählt. Es wird später mehr darauf eingegangen. 

### Fruits-360

Dieser Datensatz besteht aus 90483 Obst-Bilder, die in 131 Klassen (Avocado, Apfel, Kirschen etc.) unterteilt sind. Diese ganze Bilder würden in 3 Verzeichnisse verteilt, das erste enthält Bilder für das Training (67692 Bilder), das nächste enthält Bilder für das Testen (22688) und das letzte 103 Bilder auf denen mehreren Obst zu sehen sind. Das letztere Verzeichnis wird jedoch während dieser Arbeit nicht verwendet. Die Bilder haben eine Größe von 100x100 Pixel und der Datensatz wurde für das letzte Mal am 18. Mai 2020 aktualisiert. 

### Ähnliche Arbeiten 

Es gibt auf Kaggle eine Menge Arbeiten, die auf diesem Datensatz basiert und es wurde schon eine Genauigkeit von 98% erreicht. Aus diesem Grund ist der Fokus dieser Arbeit nicht eine bessere Accuracy zu erreichen sondern Model zu trainieren mit unterschiedlichen Parametern und zu beobachten wie die ausgewählte Parameter auf das Ergebnis einwirken und falls ungewollte Fehler auftreten, diese zu korrigieren.

### Transfer Learning 

Bei **Transfer Learning** wird ein schon trainiertes Model für eine spezifische Tätigkeit verwendet und dieses auf eine ähnliche Tätigkeit angewendet.
Diese Optimierung ermöglicht es bei der neuen Tätigkeit eine schnelle Lösung und öfter eine bessere Lösung für erreichen.
Diese Methode basiert auf 3 Schritte when man ein schon trainiertes Model weiterverwenden will: 
  - Base Model auswählen: ein schon trainiertes Model soll ausgewhählt werden, am bestens ein Model, das schon mit ähnlichen Daten wie die neuen Daten trainiert         wurde. 
  - Wiederverwendung des ausgewählten Model: das ausgewählte Model kann dann für die neue Tätigekeit eingesetzt werden. Bei dem Einsatz kann das ganze Model ohne 
    weitere Änderung oder mit Änderungen verwendet werden.
  - Bei dem letzten Schritt geht es darum, das mödel zu verbessern, um ein besseres Ergebnis zu erreichen. 

Transfer Learning ist nützlich wenn der Entwickler Zeit sparen möchte, nicht genug Daten hat und eine bessere Perfotmanz erzielen möchte. 

### ResNet50 

Da Tranfer learning alsLösungsansatz ausgewählt wurde, wird ResNet50 als Base-Model für diese Arbeit eingesetzt.

ResNet50 ist eine CNN bestehend aus 50 Layers. Das Frameworks keras stellt ein schon trainiertes Model von ResNet50 zur Verfügung, dieses Model wurde mit dem Datensatz **ImageNet** trainiert. Dieses erzielte eine Top-1 Genauigkeit von 75% und eine Top-5 Genauigkeit von 92%.













    
