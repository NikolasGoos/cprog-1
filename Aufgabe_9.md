# Aufgabe 9

Erstellen und testen Sie ein Programm, das für eine beliebige Ganzzahl die nächsthöhere gerade Zahl ausgibt. Falls die Zahl bereits gerade ist, ist die Zahl selbst auszugeben. 
Die Zahl ist durch den Benutzer einzugeben.

## Teil 1

  
  Erstellen Sie hierzu folgende Unterprogramme
  
  >void eingeben (int*)
  >
_Erhält einen Zeiger auf eine Zahl und ermöglicht die Eingabe dieser Zahl durch die Tastatur._

>void korrigieren (int*)
>
_Erhält einen Zeiger auf die vorher eingegeben Zahl und korrigiert diese, falls sie ungerade ist._

>void ausgeben (int*)
>
_Erhält einen Zeiger auf die vorher eingegebene und korrigierte Zahl und gibt diese mit Wert und Adresse am Bildschirm aus._

Testen Sie Ihr Programm mit unterschiedlichen Testfällen.

## Beispiel Pointer
<details>
<summary>Click to expand</summary>

  In dem folgenden Beispiel wird ein Pointer an ein Unterprogramm übergeben und in diesem Unterprogramm wird der eingelesen Wert direkt an die in der main deklarierten Variable gespeichert.
  ![Screenshot (37)](https://user-images.githubusercontent.com/79829648/119266126-d2013280-bbe9-11eb-9bcf-8f5c2fb8c82f.png)
An der Ausgabe kann das nachvefolgt werden.
  
  ## Ausführlich
  <details>
<summary>Click to expand</summary>
  Sie werden einen Programmcode sehen, welcher ähnlich dem zu dieser Aufgabe ist.
  Der Code, den Sie auf den Bildern sehen, bearbeitet die folgenden Punkte:
  
  - [ ] Buchstabe einlesen
  - [ ] Buchstabe verändern
  - [ ] Buchstabe ausgeben

Im ersten Punkt mit "Buchstabe einlesen", ist noch eine Fehlerabfrage eingebaut, welche vom Verständnis etwas schwierigerer ist. In den Kommentaren steht dazu aber genug.

# Main
![Screenshot (31)](https://user-images.githubusercontent.com/79829648/117532858-e9d19780-afe9-11eb-8998-6357607d014e.png)

# Buchstaben einlesen
![Screenshot (32)](https://user-images.githubusercontent.com/79829648/117532867-f2c26900-afe9-11eb-8734-7e47b38f4da7.png)

# Buchstaben verändern
![Screenshot (33)](https://user-images.githubusercontent.com/79829648/117532872-f7871d00-afe9-11eb-9e77-71b95c358ac3.png)

# Buchstaben ausgeben
![Screenshot (34)](https://user-images.githubusercontent.com/79829648/117532875-fa820d80-afe9-11eb-85b4-f26a4f26048d.png)


  
  </details>
  </details>

## Zusatz
<details>
<summary>Click to expand</summary>
  
  Erstellen Sie das Struktogramm für Ihr Hauptprogramm und für die Unterfunktionen
  </details>

  
  ## Teil 2

  
  Erweitern Sie Ihr Programm um eine weiter Funktion, die überprüft, ob die eingegebene Zahl mindestens 5-stellig ist und diese bei Bedarf korrigiert.
  
  _korrigieren2_ soll nach der Funktion aus Teil 1 aufgerufen werden.
  Füllen Sie dazu die fehlenden Stellen **rechts** neben der Zahl mit 0 auf.
