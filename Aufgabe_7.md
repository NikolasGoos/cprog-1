# Aufgabe 7

Sie suchen für Ihr Projekt einen Widerstand. Sie haben den Baukasten der E12 Reihe mit den Widerständen von 1 bis 10.000.
Um den richtigen Widerstand zu finden etwickeln Sie ein Programm, das mit hilfe der E12 Reihe den passenden Widerstand durch eine Parallelschaltung ermittelt und ausgibt.
Ihr Programm soll die folgenden Punkte erfüllen:  
  
  - [ ] Berechnen Sie die E12 Reihe bis 10.000 Ohm und geben Sie diese aus
  - [ ] Erstellen Sie eine Funktion zur Berechnung von Parallelwiderständen
    - [ ] Testen Sie Ihre Unterfunktion mit zwei Werten  
  - [ ] Berechnen Sie jede mögliche Kombination von zwei parallel geschalteten Widerständen der E12-Reihe
  - [ ] Speichern Sie die Kombination mit der kleinsten Differenz zum Wunschwiderstand
  - [ ] Geben Sie die gefundene Kombination von Widerständen aus
  - [ ] Ermittelt Sie die Abweichung in Ohm und %, und geben Sie diese aus.
  
  
# Info E12
 
 Die E12-Reihe ist eine Widerstandsreihe, welche pro Dekade eine Logarithmische verteilung aufweißt.
 Sie hat pro Dekate 12 Widerstandswerte, die sich von Dekade zu Dekade lediglich um den Faktor 10 unterschieden.
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
  > int iZähle1r=0;
  > int iZähler2=0;
  > 
  > // Doppelte for-Schleife mit den Schleifenvariablen i und k
  > 
  > for(i=0;i<4;i++){
  > 
  >   for(k=0;k<4;k++){
  >   
  >     iZähler++;
  >     
  >   }
  >   
  >   iZähler2+=2;
  >   
  > }
  > 
  > 
Für i=0 wird in die äußere Schleife gegangen, in dieser steht eine zweite Schleife mit der Schleifenvariable k.
Zuerst wird die "k"-Schleife durchlaufen, in deisem Beispiel wird iZähler1 jedes mal um 1 erhöht, bis diese Verlassen wird.
Danach wird iZähler2 um 2 erhöht, damit ist die "i"-Schleife zu enden und i wird um 1 erhöht, wenn die bedingung für i (hier i<4) erfüllt ist dann wird die "i"-Schleife erneut durchlaufen.
Dies wird widerholt, bis i=4 ist und die Bedingung i<4 nicht mehr erfüllt wird, da die äußere Schleife verlassen wird. 

</details>
  


## Tip - Widerstände speicher

<details>
 <summary>Click to expand</summary>

  
   Berechen die Differenz zwischen dem aktuellen Widerstand und dem Wunschwiderstand. Achte dabei auch auf das Vorzeichen.
   Ist der aktuelle Widerstand näher an dem gewünschten Widerstand als der zuletzt gespeicherte, speicher die neuen Werte.
   Es können die Schleifenvariablen gespiechert werden, da über diese, der Aktuelle Widerstand ermittelt werden kann.
   Es können auch die ermittelten Widerstände gespeichert werden.

  </details>
