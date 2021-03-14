## System detekcji

Ostatnimi czasy, członkowie koła AGH Solar Plane postanowili, że chcą tchnąć odrobinę inteligencji w swoje samoloty. Plany były wielkie, stworzyć sztuczną inteligencję będącą w stanie rozpoznawać wszystko co zobaczy. Jednakże ich pierwotne marzenia zostały rozsypane, gdy dowiedzieli się, że związku z panującą epidemią _COVID-19_ dotację na koła naukowe zostały drastycznie obcięte. 

Ich pierwotne ambicje o stworzeniu sieci neuronowych musiały zostać odłożone na bok, a problem rozwiązany prostszymi metodami. Postawiono na prosty algorytm detekcji na podstawie rozmiaru obiektu. Pozostali członkowie koła przygotowali już pierwsze segmenty detekcji, pozostawiając Tobie najbardziej kluczowy z nich. 

Otrzymując uproszczony już obraz z kamery pokładowej w postaci macierzy ___X___ x ___Y___ o wartościach 0 lub 1, gdzie 1 oznacza kolor _krowopodobny_, zaś 0 kolor _trawopodobny_ twój algorytm musi odnaleść wszystkie krówki widoczne na kamerze.

Plamy krowopodobne są zawsze tylko pionowymi lub poziomymi liniami. Twój algorytm ma na podstawie rozmiaru plamy decydować o przynależności obiektu do klasy krów. Możemy powiedzieć, że _plama jest krową_, gdy jej rozmiar wynosi 2 lub 3 pola.

---

## Wejście

Na wejściu twój program otrzmuje w pierwszej linii liczby ___X___ oraz ___Y___ oznaczające szerokość oraz wysokość klatki obrazu. Następne ___Y___ linii zawiera po ___X___ 0 lub 1.

--- 

## Wyjście

Na wyjściu twój program w pierwszej i jedynej linii podać liczbę znalezionych krówek.

--- 

## Przykładowe dane

Dla danych wejściowych
```
8 8
0 0 0 0 0 0 0 0
0 1 1 1 1 0 0 0
0 0 0 0 0 0 0 0
0 0 0 1 1 1 1 0
0 0 0 0 0 0 0 0
0 0 0 0 0 1 1 0
0 0 0 1 0 0 0 0
0 0 0 1 0 0 0 0
```

Poprawnym wynikiem jest

```
2
```

### Wyjaśnienie

Na obrazie znajdują się 4 plamy o rozmiarach 4, 4, 2, 2. Jedynie plamy o rozmiarze 2 lub 3 są zaliczanie do krów.
