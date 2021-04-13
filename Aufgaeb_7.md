# Aufgabe 7


  Etwickeln Sie ein Programm, das mit hilfe der E12 Reihe den passenden Widerstand mit hilfe einer Parallelschaltung sucht und berechnet.
  
  - [ ] E12 Reihe
  - [ ] Parallelschaltung
  - [ ] Widerständefinden
  - [ ] Widerstände speicher
  
  
  
## Die E12 Reihe

Schreibe eine Unterfunktion, die einen Integerwert übergeben bekommt und den E12 Widerstand (als float) zurück gibt.

Die E12 Reihe sind Widerstände, die 12 Widerstände pro Dekade erhalten !

  - [x] E12 Reihe
  - [ ] Parallelschaltung
  - [ ] Widerständefinden
  - [ ] Widerstände speicher


  
  ## Parallelschaltung
  
  Schreibt eine zwietes Unterprogramm, welches zwei Werte übergeben bekommt, aus diesen den Parallelwiderstand berechnet und das Ergebniss zurück gibt.
  
  - [x] E12 Reihe
  - [x] Parallelschaltung
  - [ ] Widerständefinden
  - [ ] Widerstände speicher
  
  
  ## Wiederstände finden
  
  Der Benutzer soll vor der Ausführung aufgefordert Werden den gesuchten Widerstand anzugeben.
  Schrieben Sie in der main einen Code, welcher für die E12 Reihe bis 10.000 Ohm den Parallelwiderstand jeder möglichen komnbination berechnet.
  
  
 - [x] E12 Reihe
 - [x] Parallelschaltung
 - [x] Widerständefinden
 - [ ] Widerstände speicher


## Widerstände speicher

Erweiter dein Programm so, dass die Widerstandswerte gespeichert werden, wenn sie am dichtesten an dem gewünschten Wert sind.


 - [x] E12 Reihe
 - [x] Parallelschaltung
 - [x] Widerständefinden
 - [x] Widerstände speicher

### Tip 1


<summary>Click to expand</summary>
  
   Benutze pow() mit 10 hoch x/12
  

### Tip 2

<details>
  
<summary>Click to expand</summary>
  
   Die Parallelschaltung kann als a*b/(a+b) realisiert werden
  
  <details>
  
  ### Tip 3
  
<details>
  
  <summary>Click to expand</summary>
   Benutze eine doppelte Schleiche, welche die beiden Unterfunktionen aufruft.
  
<details>
  
  
  ### Tip 4
  
<details>
  
 <summary>Click to expand</summary>
  
   Berechen die Differenz zwischen dem letzten und aktuellen Widerstand im vergleich zum gewünschten Widerstand, speichere den besseren.
   Speicher den Zähler und übergib ihn am Ende wieder der passenden Unterfunktion, um den ermittelten Widerstand zu bestimmen.
   Überprüfe ob die Differenz negativ ist
    
  
  

  <details>
