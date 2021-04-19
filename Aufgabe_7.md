# Aufgabe 7

Sie suchen für Ihr Projekt einen Widerstand. Sie haben den Baukasten der E12 Reihe mit den Widerständen von 1 bis 10.000.
Leider ist kein Widerstand dabei, der nah genug an ihrem Wunschwert liegt. Sie möchten dem durch 2 parallel geschaltete Widerstände aus der E12 Reihe möglichst nahe kommen.  Entwickeln Sie ein Programm, das alle Kombinationen automatisch erstellt und das beste Widerstandspaar für Sie ermittelt und ausgibt.
Ihr Programm soll die folgenden Punkte erfüllen:  
  
  - [ ] Berechnen Sie die E12 Reihe bis 10.000 Ohm und geben Sie diese aus
  - [ ] Erstellen Sie eine Funktion zur Berechnung von Parallelwiderständen
    - [ ] Testen Sie Ihre Unterfunktion mit zwei Werten  
  - [ ] Berechnen Sie jede mögliche Kombination von zwei parallel geschalteten Widerständen der E12-Reihe
  - [ ] Speichern Sie die Kombination mit der kleinsten Differenz zum Wunschwiderstand
  - [ ] Geben Sie die gefundene Kombination von Widerständen aus
  - [ ] Ermitteln Sie die Abweichung in Ohm und Prozent und geben Sie diese aus
  
  
# Info E12
 
 Die E12-Reihe ist eine Widerstandsreihe, welche eine logarithmische Verteilung aufweist.
 Sie hat pro Dekade 12 Widerstandswerte, die sich von Dekade zu Dekade lediglich um den Faktor 10 unterscheiden.
 Wie sich die E12-Reihe berechnen lässt kann unter dem Wikipedia-Link nachgelesen werden
 
 Wiki:
 https://de.wikipedia.org/wiki/E-Reihe
 

  
## Tip - E12 Reihe

<details>
<summary>Click to expand</summary>

Die E12 Reihe sind Widerstände, die 12 Widerstände pro Dekade erhalten !
Geben Sie die E12-Reihe von 1 bis 10.000 an

Es kann die Funktion pow() mit 10 hoch x/12 verwendet werden.
pow() befindet sich in der math.h Bibliothek

 </details>
  
  ## Tip - Parallelschaltung
  
  <details>
  <summary>Click to expand</summary>
  
  Die Parallelschaltung kann durch 
  
  >R1*R2/(R1+R2)
  >
 
   realisiert werden.
  
  </details>

  
 ## Tip - Wiederstände berechnen
  
  <details>
  <summary>Click to expand</summary>

 Um alle Widerstandskombinationen zu brechnen kann eine doppelte for-Schleife verwendet werden 
  
  Beispiel:
  
  > int i=0;
  > int k=0;
  > int iZaehler1=0;aehler2=0;
  > 
  > // Doppelte for-Schleife mit den Schleifenvariablen i und k
  > 
  > for(i=0;i<4;i++){
  > 
  >   for(k=0;k<4;k++){
  >   
  >     iZaehler1++;
  >     
  >   }
  >   
  >   iZaehler2+=2;
  >   
  > }
  > 
  > 
Die erste For-Schleife ist die äußere Schleife mit Schleifenvariable i. In dieser ist eine zweite Schleife mit der Schleifenvariable k enthalten.
Zuerst wird die innere "k"-Schleife 4 mal durchlaufen, in diesem Beispiel wird iZaehler1 dabei jedes mal um 1 erhöht.
Danach wird iZaehler2 um 2 erhöht. Anschließend ist ist die "i"-Schleife zu Ende und i wird um 1 erhöht, solange i kleiner 4 ist. Anschließend die "i"-Schleife erneut durchlaufen.
Dies wird widerholt, bis i=4 ist und die Bedingung i<4 nicht mehr erfüllt wird. Die äußere Schleife wird verlassen. 

</details>
  


## Tip - Widerstände speichern

<details>
 <summary>Click to expand</summary>

  
   Berechnen Sie die Differenz zwischen dem aktuellen Widerstand und dem Wunschwiderstand. Achten Sie dabei auch auf das Vorzeichen.
   Ist der aktuelle Widerstand näher an dem gewünschten Widerstand als der zuletzt gespeicherte, dann speichern Sie die neuen Werte.
   Es sollten auch die Schleifenvariablen gespeichert werden, da über diese der aktuelle Widerstand ermittelt werden kann.
   Es können auch die ermittelten Widerstände gespeichert werden.

  </details>
