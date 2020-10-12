# Bubblesort

## Ausgangslage
Gegeben ist ein unsortiertes Array mit *n* Elementen, das sortiert werden soll.

## Ablauf
In einer Schleife wird jedes Element eines Feldes mit seinem rechten Nachbarn
verglichen. Wenn das Sortierkriterium verletzt wird, werden die beiden Elemente
vertauscht. Am Ende der Vertauschungsphase steht je nach Sortierung (aufsteigend
oder absteigend) entweder das größte oder das kleinste Element der Eingabe am
Ende der Liste. Diese Vertauschungen werden solange wiederholt, bis die
Eingabeliste vollständig sortiert ist. Das letzte Element des vorherigen
Durchlaufs muss dabei jeweils nicht mehr betrachtet werden, da in den restlichen
Elementen keines mehr enthalten ist, das größer bzw. kleiner ist.

## Zeitkomplexität

### Ungünstigster Fall
Bubblesort hat im schlechtesten Fall die Laufzeit $O(n^2)$.

### Bester Fall
Im besten Fall ist das vorliegende Array bereits sortiert und Bubblesort wird
die Liste nur einmal durchgehen, um festzustellen, dass die Liste bereits sortiert
ist, weil keine benachbarten Elemente vertauscht werden mussten. Die Zeitkomplexität
liegt in diesem Fall bei $O(n)$.

### Durchschnittlicher Fall
Die durchschnittliche Laufzeit ist $O(n^2)$.

## Speicherkomplexität
Bubblesort ist ein in-place arbeitender Algorithmus, dass heißt, dass kein
zusätzlicher Speicherplatz benötigt wird.

## Beispiel

```
arr[] = {10, 80, 40, 30}
Indexe:  0   1   2   3

1. Index = 0, Zahl = 10
2. 10 < 80, es wird nicht getauscht

3. Index = 1, Zahl = 80
4. 80 > 40, vertausche 80 und 40
5. Die neue Sortierung des Array ist {10, 40, 80, 30}

6. Index = 2, Zahl = 80
7. 80 > 30, vertausche 80 und 30
8. Die neue Sortierung des Array ist {10, 40, 30, 80}

  Die Liste wird ein weiteres Mal durchgegangen, das letzte Element des
  Array wird dabei nicht mehr betrachtet.

arr[] = {10, 40, 30, 80}
Indexe:  0   1   2   3

1. Index = 0, Zahl = 10
2. 10 < 40, es wird nicht getauscht

3. Index = 1, Zahl = 40
4. 40 > 30, vertausche 40 und 30
5. Die neue Sortierung des Array ist {10, 30, 40, 80}

6. Index = 2, Zahl = 40
7. 40 < 80, es wird nicht getauscht
8. Die neue Sortierung des Array ist {10, 30, 40, 80}

  Die Liste wird ein weiteres Mal durchgegangen, das vorletzte Element des
  Array wird dabei nicht mehr betrachtet.

arr[] = {10, 30, 40, 80}
Indexe:  0   1   2   3

1. Index = 0, Zahl = 10
2. 10 < 30, es wird nicht getauscht

3. Index = 1, Zahl = 30
4. 30 < 40, es wird nicht getauscht

5. Index = 2, Zahl = 40
6. 40 < 80, es wird nicht getauscht

  Da im letzten Durchlauf gar nicht getauscht wurde, ist das Array
  jetzt sortiert.
```

## Implementierungen
- [Java](https://github.com/TheAlgorithms/Java/blob/master/Sorts/BubbleSort.java)
- [Java - Rekursiv](https://github.com/TheAlgorithms/Java/blob/master/Sorts/BubbleSortRecursion.java)
- [Javascript](https://github.com/TheAlgorithms/Javascript/blob/master/Sorts/BubbleSort.js)
- [C++](https://github.com/TheAlgorithms/C-Plus-Plus/blob/master/sorting/bubble_sort.cpp)
- [Rust](https://github.com/TheAlgorithms/Rust/blob/master/src/sorting/bubble_sort.rs)
- [Python](https://github.com/TheAlgorithms/Python/blob/master/sorts/bubble_sort.py)
- [Dart](https://github.com/TheAlgorithms/Dart/blob/master/sort/bubble_Sort.dart)
- [PHP](https://github.com/TheAlgorithms/PHP/blob/master/sorting/bubbleSort.php)
- [Haskell](https://github.com/TheAlgorithms/Haskell/blob/master/src/Sorts/BubbleSort.hs)
- [MATLAB/Octave](https://github.com/TheAlgorithms/MATLAB-Octave/blob/master/algorithms/sorting/bubble_sort.m)
- [Kotlin](https://github.com/TheAlgorithms/Kotlin/blob/master/src/main/kotlin/sort/BubbleSort.kt)
- [Scala](https://github.com/TheAlgorithms/Scala/blob/master/src/main/scala/Sort/BubbleSort.scala)
- [C](https://github.com/TheAlgorithms/C/blob/master/sorting/bubble_sort.c)
- [C - Rekursiv](https://github.com/TheAlgorithms/C/blob/master/sorting/bubble_sort_recursion.c)
- [Go](https://github.com/TheAlgorithms/Go/blob/master/sorts/bubblesort.go)
- [R](https://github.com/TheAlgorithms/R/blob/master/sorting/Bubble%20sort.R)
- [Ruby](https://github.com/TheAlgorithms/Ruby/blob/master/Sorting/bubble_sort.rb)

## Videos
- [Bubble-sort with Hungarian ("Csángó") folk dance](https://www.youtube.com/watch?v=lyZQPjUT5B4)

## Weitere Informationen
- Bubblesort wird auch "Sortieren durch Aufsteigen" oder "Austauschsortieren"
  genannt
