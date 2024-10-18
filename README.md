
# `less` – Opis polecenia

`less` to polecenie w systemie Linux służące do przeglądania plików tekstowych w trybie stronicowania. Pozwala na przewijanie pliku w górę i w dół, w przeciwieństwie do komendy `more`, która umożliwia jedynie przewijanie w dół. `less` jest bardziej elastyczny i oferuje dodatkowe funkcje do poruszania się po plikach.
```bash
less [opcje] [plik]
```
## Argumenty polecenia:
#### `-N`: Wyświetla numery linii
```bash
less -N nazwa_pliku.txt
```
#### `-S`: Wyłącza automatyczne zawijanie linii (przydatne przy długich liniach)
```bash
less -S nazwa_pliku.txt
```
#### `-p`: "wzorzec" - Otwiera plik i przeskakuje do pierwszego wystąpienia wzorca tekstowego
```bash
less -p "szukany_tekst" nazwa_pliku.txt
```
#### `+F`: Włącza tryb automatycznego przewijania (follow mode)
```bash
less +F nazwa_pliku.txt
```
<hr>
