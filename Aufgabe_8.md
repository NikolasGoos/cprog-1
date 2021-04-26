# Aufgabe 8

Diese Aufgabe führt Sie Schritt für Schritt an das Thema Unterfunktionen und Arrays heran.
Sie müssen daher nicht für jeden Teil eine neue Datei anlegen, sondern erweitern oder verändern Sie die zuletzt verwendete den Aufgaben entsprechend.

## Teil 1
<details>
<summary>Click to expand</summary>

Erstellen Sie ein Feld von 10 int-Werten und Initialisieren Sie das Feld mit beliebigen Daten.
Berechnen Sie die Summe aller Feldelemente und geben Sie die Summe aus.
Berechnen Sie den Mittelwert aller Feldelemente und geben Sie diesen aus.
Ermitteln Sie das größte Feldelement und geben Sie dessen Position und Wert aus.
Das alles soll in der Hauptfunktion geschrieben werden.

Hier nochmal in Kurzform:
- [ ] Feld Initialisieren
- [ ] Summe berechnen
- [ ] Mittelwert berechnen
- [ ] Größtes Feldelement suchen




### Tip 1 - Summeberechnen
<details>
<summary>Click to expand</summary>
  
Berechnen Sie Summe des Feldes mit der Hilfe einer for() oder while() Schleife.


</details>



### Tip 2 - Feldelement
<details>
<summary>Click to expand</summary>

Lassen Sie eine Zählschleife laufen und überprüfe, welcher Wert kleiner bzw. größer ist und speichern Sie den Wert und die Stelle zum Beispiel in einer Hilfsvariable ab.

</details>

</details>



## Teil 2

<details>
<summary>Click to expand</summary>

Ihr Programm soll nun so erweitert/verändert werden, dass die unten aufgelisteten Aufgaben in Unterfunktionen stehen.

- [ ] Summe berechnen
- [ ] Mittelwert berechnen
- [ ] Größtes Feldelement und Stelle suchen

Die Unterfunktionen sollten diese Form aufweisen:
>  int summe (int [10])
>  

> float mittelwert (int [10])
> 

> int maximum (int [10], int*)
> 

</details>


## Teil 3

<details>
<summary>Click to expand</summary>
  Erweitern Sie nun Ihr Programm um die aufgelistetn Aufgaben.
  Diese sollen ebenfalls als Unterfunktionen in Ihrem Programm stehen.
  

### Feld einlesen
  
  Der Benutzer soll ein beliebiges 10er Feld (Integer)
  (siehe Aufgabe 8, Teil 1) über die Tastatur eingeben können.
  
  > void feld_einlesen(int [10])
  > 


### Feld ausgeben

Entwickeln Sie ein Unterprogramm, um ein 10er Feld am Bildschirm anzeigen zu können.

>void feld_ausgeben (int [10])
>

### Feld berechenen

Berechnen Sie für das vom Benutzer eingegebene Feld die Summe, den Mittelwert, das größte Feldelement und zeigen Sie das Feld an.
Benutzen Sie dafür die Unterprogramme aus 8.2


  </details>
  
  
  ## Teil 4

<details>
<summary>Click to expand</summary>
  
  Erweitern Sie Ihr Programm um ein weiteres Unterprogramm, welches das Feld sortiert.
  
  > void feld_sortieren (int[10])
  > 

Geben Sie das Feld vor und nach dem sortieren aus.


### Tip 1 (Info) - Felder sortieren
<details>
<summary>Click to expand</summary>
_Sortieren von Feldern ist ein ganz wichtiger Bestandteil der Programmierung. 
Zu diesem Thema gibt es gleich eine ganze Reihe an Verfahren, die sich in Komplexität und
Geschwindigkeit sehr unterscheiden._

Der hier vorgestellte Algorithmus ist der 'Selection-sort'.
Der Algorithmus ist vergleichsweise langsam, aber einfach.
Es werden 2 ineinander geschachtelte Schleifen verwendet.

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
  </details>
