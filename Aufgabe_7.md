# Aufgabe 7

 Ihr sucht für eure Schaltung einen Widerstand. In eurem Baukasten ist aber nur die E12 Reihe von 1 bis 10.000 vorhanden.
 Entwickeln Sie ein Programm, das mit Hilfe der E12 Reihe den passenden Widerstand durch eine Parallelschaltung näherungsweise berechnet und
 angibt, welche Widerstände benötigt werden.
  
  - [ ] E12 Reihe
  - [ ] Parallelschaltung
  - [ ] Widerstände finden
  - [ ] Widerstände speichern
  
  
  
## Die E12 Reihe

<details>
<summary>Click to expand</summary>
  
Schreibe eine Unterfunktion, die einen Integerwert übergeben bekommt und den E12 Widerstand (als float) zurück gibt.

Die E12 Reihe sind Widerstände, die 12 Widerstände pro Dekade erhalten!

  - [x] E12 Reihe
  - [ ] Parallelschaltung
  - [ ] Widerstände finden
  - [ ] Widerstände speichern

### Tip 1

<details>
<summary>Click to expand</summary>
  
   Benutze pow() mit 10 hoch x/12
  </details>
 </details>
  
  ## Parallelschaltung
  
  <details>
<summary>Click to expand</summary>
  Schreibt eine zweites Unterprogramm, welches zwei Werte übergeben bekommt, aus diesen den Parallelwiderstand berechnet und das Ergebnis zurückgibt.
  
  - [x] E12 Reihe
  - [x] Parallelschaltung
  - [ ] Widerständefinden
  - [ ] Widerstände speichern
  
  ### Tip 2

<details>
<summary>Click to expand</summary>
  
   Die Parallelschaltung kann als a*b/(a+b) realisiert werden
  
  </details>
   </details>
  
  ## Widerstände finden
  
  <details>
  <summary>Click to expand</summary>
  
  Der Benutzer soll vor der Ausführung aufgefordert Werden den gesuchten Widerstand anzugeben.
  Schreiben Sie in der main einen Code, welcher für die E12 Reihe bis 10.000 Ohm den Parallelwiderstand jeder möglichen Kombination berechnet.
  
  
 - [x] E12 Reihe
 - [x] Parallelschaltung
 - [x] Widerstände finden
 - [ ] Widerstände speichern

  ### Tip 3
  
<details>
  <summary>Click to expand</summary>
   Benutze eine doppelte Schleife, welche die beiden Unterfunktionen aufruft.
  
</details>
</details>
  


## Widerstände speicher

<details>
 <summary>Click to expand</summary>

Erweiter dein Programm so, dass die Widerstandswerte gespeichert werden, wenn sie am dichtesten an dem gewünschten Wert sind.


 - [x] E12 Reihe
 - [x] Parallelschaltung
 - [x] Widerstände finden
 - [x] Widerstände speicher


  
  ### Tip 4
  
  <details>
 <summary>Click to expand</summary>
  
   Berechne die Differenz zwischen dem letzten und aktuellen Widerstand im Vergleich zum gewünschten Widerstand, speichere den besseren.
   Speicher den Zähler und übergib ihn am Ende wieder der passenden Unterfunktion, um den ermittelten Widerstand zu bestimmen.
   Überprüfe, ob die Differenz negativ ist.
    
  
   </details>

  </details>

## Zusatz

<details>
 <summary>Click to expand</summary>
  
  Bitte erst dann weiter machen, wenn alles zuvor funktioniert!

### Let's Go
<details>
 <summary>Click to expand</summary>
 
 Du kannst nun 3 Widerstände für deinen gesuchten Widerstand benutzen und beliebig anordnen.
 Schriebe dein Programm so um, dass die gegebene E12 Reihe den gesucht Widerstand aus allen möglichen Kombinationen die beste Kombination berechnet.
 Die Widerstandswerte und die verwendete Kombination sind am Ende auf dem Bildschirm auszugeben.
 
 </details>
  </details>

