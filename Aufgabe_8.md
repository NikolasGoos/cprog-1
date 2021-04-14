# Aufgabe 8

## Teil 1
<details>
<summary>Click to expand</summary>

Erstellen Sie ein Feld von 10 int-Werten und Initialisieren se das Feld mit beliebigen Daten.
Berechnen Sie die Summe aller Feldelemente und geben Sie die Summe aus.
Berechnen Sie den Mittelwert aller Feldelemente und geben Sie diesen aus.
Ermitteln Sie das größte Feldelement und geben sie dessen Position und Wert aus.

- [ ] Feld Initialisieren
- [ ] Summe berechnen
- [ ] Mittelwert berechnen
- [ ] Größtes Feldelement suchen


### Schritt 1

Initialisiere ein Integer-Feld mit 10 beliebigen Zahlenwerten

- [x] Feld Initialisieren
- [ ] Summe berechnen
- [ ] Mittelwert berechnen
- [ ] Größtes Feldelement suchen


### Schritt 2

Berechne die Summe des Feldes mit hilfe einer for() oder while() Schleife als Unterfunktion.
Die Summe soll auf dem Bildschirm ausgegeben werden.

- [x] Feld Initialisieren
- [x] Summe berechnen
- [ ] Mittelwert berechnen
- [ ] Größtes Feldelement suchen


### Schritt 3

Die Mittelwertberechnung soll ebenfalls als Unterfunktion geschrieben werden, welche die Unterfunktion für die Summe in sich aufruft.
Der Mittelwert soll auf dem Bildschirm ausgegeben werden.

- [x] Feld Initialisieren
- [x] Summe berechnen
- [x] Mittelwert berechnen
- [ ] Größtes Feldelement suchen


### Schritt 4

Schreiben Sie eine Schleife, welchen aus ihrem Feld das größte Element und dessen Position in dem Feld ermittelt und ausgibt.
Sie können dafür eine Unterfunktion verwenden oder es direkt in der Haptfunktion schreiben.

- [x] Feld Initialisieren
- [x] Summe berechnen
- [x] Mittelwert berechnen
- [x] Größtes Feldelement suchen

### Tip (Schritt 4)
<details>
<summary>Click to expand</summary>

Lass eine Zählschleife laufen und überprüfe welcher Wert kleiner bzw größer ist.

</details>

</details>



## Teil 2

<details>
<summary>Click to expand</summary>

Strukturieren sie ihr Programm mit den folgenden Unterprogrammen

- [ ] Summe berechnen
- [ ] Mittelwert berechnen
- [ ] Größtes Feldelement suchen

>  int summe (int [10])
>  
Berechnung der Summe aller Elemente des übergebene Feldes int [10]     

- [x] Summe berechnen
- [ ] Mittelwert berechnen
- [ ] Größtes Feldelement suchen


> float mittelwert (int [10])
> 
Berechnung des Mittelewrts aller Elemente des übergebenen Feldes int [10]

- [x] Summe berechnen
- [x] Mittelwert berechnen
- [ ] Größtes Feldelement suchen

> int maximum (int [10], int*)
> 
Suche nach dem größten Feldelement und Ausgabe seiner Position (Index) im Feld.
Nutzen Sie zur übergabe des Indexein call-byreference
</details>


## Teil 3

<details>
<summary>Click to expand</summary>
  
- [ ] Feld einlesen
- [ ] Feld ausgeben
- [ ] Summe, Mittelwert, größte Feldelement

### Feld einlesen
  
  Erweiter Sie Ihr Hauptprogramm _int main ()_, damit der Benutzer ein  beliebiges 10er Feld
  (siehe Aufgabe 8, Teil 1) über die Tastatur eingeben kann.
  Schreibe dazu eine Funktion:
  
  > void feld_einlesen(int [10])
  > 

- [x] Feld einlesen
- [ ] Feld ausgeben
- [ ] Summe, Mittelwert, größte Feldelement


### Feld ausgeben

Entwickeln Sie ein Unterprogramm, um ein 10er Feld am Bildschirm anzeigen zu können.

>void feld_ausgeben (int [10])
>

Ausgabe eines 10er Feldes am Bildschirm

- [x] Feld einlesen
- [x] Feld ausgeben
- [ ] Summe, Mittelwert, größte Feldelement

### Feld berechenen

Berechnen Sie für das vom Benutzer eingegebene Feld die Summe, den Mittelwert, das größte Feldelement und zeigen Sie das Feld an.
Benutzen Sie dafür die Unterprogramme aus 8.2

- [x] Feld einlesen
- [x] Feld ausgeben
- [x] Summe, Mittelwert, größte Feldelement

  </details>
  
  
  ## Teil 4

<details>
<summary>Click to expand</summary>
  
  Erweitern Sie Ihr Programm um ein Unterprogramm, welches das Feld sortiert
  
  > void feld_sortieren (int[10])
  > 

Geben Sie das Feld vor und nach dem sortieren aus.

_Sortieren von Feldern ist ein ganz wichtiger Bestandteilder Programmiernug. 
Zu diesem Thema gibt es gleich eine gnaze Reihe an Verfahren, die sich in Komplexität und
Geschwindigkeit sehr unterscheiden._

Der hier vorgestellte Algorithmus ist der 'Selection-sort'.
Der Algorithmus ist vergleichsweise langsam, aber einfach.
Man braucht 2 ineinander geschachtzelte Schleifen.

   >   Bsp: mit 5 Werten: f[0]...f[4] enthalten 10 5 2 1 7
   >   1. Durchlauf i=0
   >   i:0    j: läuft von 1 bis 4. Falls f[j] kleiner als f[i] ist, dann tausche beide Werte
   >   i=0  j=1;  10 5 2 1 7 -> f[1]=5  <   f[0]=10 -> tasuche: 5 und 10
   >   i=0  j=2;  5 10 2 1 7 -> f[2]=2  <   f[0]=5 -> tasuche: 5 und 2
   >   i=0  j=3;  2 10 5 1 7 -> f[3]=1  <   f[0]=2 -> tasuche: 2 und 1
   >   i=0  j=4;  1 10 5 2 7 -> f[4]=7  <   f[0]=1 _Nein_ -> nicht tauschen
   >   f[0] ist das kleinste Element, weiter mit den restlichen Elementen
   >
   >   2. Durchlauf i=1
   >   i:i    j: läuft von 2 bis 4. Falls f[j] kleiner als f[i] ist, dann tausche beide Werte
   >   i=1  j=2;  1 10 5 2 7 -> f[2]=5  <   f[1]=10 -> tasuche: 5 und 10
   >   i=1  j=3;  5 10 2 1 7 -> f[3]=2  <   f[1]=2 -> tasuche: 5 und 2
   >   i=1  j=4;  2 10 5 1 7 -> f[4]=7  <   f[1]=2 _Nein_ -> nicht tauschen
   >   f[0] und f[1] sind sortiert, weiter mit dem Rest
   >   ........... 

  
  
  </details>
