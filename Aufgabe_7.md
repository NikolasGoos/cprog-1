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

Benutze die Funktion pow() mit 10 hoch x/12.
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
  
  Beispiel mit den Widerständen R1, R2, R3, R4:
  
  > R1||R1
  > R1||R2
  > R1||R3
  > R1||R4
  > 
  > R2||R1
  > R2||R2
  > R2||R3
  > .............
  > R4||R3
  > R4||R4
  > 


</details>
  


## Widerstände speicher

<details>
 <summary>Click to expand</summary>

Erweiter dein Programm so, dass die Widerstandswerte gespeichert werden, wenn sie am dichtesten an dem gewünschten Wert sind.


 - [x] E12 Reihe
 - [x] Parallelschaltung
 - [x] Widerständefinden
 - [x] Widerstände speicher


  
  ### Tip 4
  
  <details>
 <summary>Click to expand</summary>
  
   Berechen die Differenz zwischen dem letzten und aktuellen Widerstand im vergleich zum gewünschten Widerstand, speichere den besseren.
   Speicher den Zähler und übergib ihn am Ende wieder der passenden Unterfunktion, um den ermittelten Widerstand zu bestimmen.
   Überprüfe ob die Differenz negativ ist
    
  
   </details>

  </details>
