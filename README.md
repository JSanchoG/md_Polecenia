
# `less` – Opis polecenia

`less` to polecenie w systemie Linux służące do przeglądania plików tekstowych w trybie stronicowania. Pozwala na przewijanie pliku w górę i w dół, w przeciwieństwie do komendy `more`, która umożliwia jedynie przewijanie w dół. `less` jest bardziej elastyczny i oferuje dodatkowe funkcje do poruszania się po plikach.
```bash
$ less [opcje] [plik]
```
## Argumenty polecenia:
#### `-N`: Wyświetla numery linii
```bash
$ less -N nazwa_pliku.txt
```
Przykład polecenia:
```bash
$ less -N test.txt
```
![](https://i.imgur.com/zfTAVkO.png)<hr>
#### `-S`: Wyłącza automatyczne zawijanie linii (przydatne przy długich liniach)
```bash
$ less -S nazwa_pliku.txt
```
Przykład polecenia:
```bash
$ less -S test.txt
```
![](https://i.imgur.com/kMaL99i.png)<hr>
#### `-p`: "wzorzec" - Otwiera plik i przeskakuje do pierwszego wystąpienia wzorca tekstowego
```bash
$ less -p "szukany_tekst" nazwa_pliku.txt
```
Przykład polecenia:
```bash
$ less -p "Luka" test.txt
```
![](https://i.imgur.com/uggMQ8i.png)

<hr>

#### `+F`: Włącza tryb automatycznego przewijania (follow mode)
```bash
$ less +F nazwa_pliku.txt
```
Przykład polecenia:
```bash
$ less +F test.txt
```
![](https://i.imgur.com/z9puhVl.png)


<hr>

## `Less` skróty klawiaturowe

#### Polecenie `less` akceptuje skróty klawiaturowe ułatwiające nawigację po tekście, zwłaszcza podczas czytania dużych plików:


    Strzałka w dół, Enter, e, j : Jedna linia do przodu.
    
    Strzałka w górę, y, k : Jedna linia wstecz.
    
    Spacja, Page Down : Jedna strona do przodu.
    
    Page Up, b : Jedna strona wstecz.
    
    Strzałka w prawo : Przewiń w prawo.
    
    Strzałka w lewo : Przewiń w lewo.
    
    Home, g : Skok na początek pliku.
    
    End, G : Skok na koniec pliku.
    
    /[string] : Wyszukiwanie w przód określonego ciągu.
    
    ?[łańcuch] : Wyszukiwanie wstecz dla określonego ciągu.
    
    n : Następne dopasowanie podczas wyszukiwania.
    
    N : Poprzednie dopasowanie podczas wyszukiwania.
    
    q : Wyjdź.



# `wc` – Opis polecenia

`wc` (word count) to polecenie w systemie Linux służące do zliczania liczby linii, słów i znaków w plikach tekstowych. Umożliwia szybkie sprawdzenie rozmiaru pliku pod kątem ilości zawartych danych.

```bash
$ wc [opcje] [plik]
```
Testowy plik `test.txt`:
```
testowy dokument
test
test
test

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut vulputate nisl consequat augue ornare vehicula quis non nibh. In vulputate lorem a purus feugiat, vel tincidunt lorem laoreet. Nam lacinia volutpat ex vel accumsan. Praesent rhoncus felis purus, ut finibus turpis malesuada eget. In vitae enim sed ante vestibulum aliquet a sed erat. Cras rutrum consectetur lectus, eu aliquet lacus lobortis id. Sed vel congue dolor, a interdum est. Nulla tincidunt erat in nisi porta finibus. Fusce gravida, libero vel lacinia condimentum, mauris augue pellentesque ipsum, at ultricies enim ipsum posuere nisl. Etiam aliquam congue lacus, eu aliquam nisl vehicula vel. Sed id orci elit. Phasellus orci turpis, auctor in nisi et, fringilla posuere diam.

Luka Doncic is Devin Booker Father.
```
## Argumenty polecenia:
#### `-l`: Wyświetla liczbę linii
```bash
$ wc -l nazwa_pliku.txt
```
Przykład polecenia:
```bash
$ wc -l test.txt 
8 test.txt
```
<hr>

#### `-w`: Wyświetla liczbę słów
```bash
$ wc -w nazwa_pliku.txt
```
Przykład polecenia:
```bash
$ wc -w test.txt 
126 test.txt
```
<hr>

#### `-c`: Wyświetla liczbę bajtów (znaków)
```bash
$ wc -c nazwa_pliku.txt
```
Przykład polecenia:
```bash
$ wc -c test.txt 
817 test.txt
```
<hr>

#### `-m`: Wyświetla liczbę znaków (również tych wielobajtowych, np. UTF-8)
```bash
$ wc -m nazwa_pliku.txt
```
Przykład polecenia:
```bash
$ wc -m test.txt 
817 test.txt
```
<hr>

#### `-L`: Wyświetla długość najdłuższej linii
```bash
$ wc -L nazwa_pliku.txt
```
Przykład polecenia:
```bash
$ wc -L test.txt 
746 test.txt
```
<hr>
