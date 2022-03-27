# Python

## Podstawy
### Operatory matematyczne
- odejmowanie - -
- dodawanie - +
- mnożenie - *
- dzielenie - /
- potęgowanie - **
- reszta z dzielenia (modulo) - %
- dzielenie bez reszty - //
### Typy danych
- liczby całkowite -	np. -2, 0, 2
- liczby zmiennoprzecinkowe	- np. -1.25, 0.0, 1.5
- stringi	- np. 'a', 'szynka', '11'
### Działania na stringach
- dodawanie stringów (konkatenacja)	 - np. a' + 'b'
- mnożenie stingów	- np. napis' * 2
### Funkcje podstawowe
- drukowanie na ekranie ciagów	- print()
- pobieranie danych przez użytkwonika -	input()
- obliczanie liczby znaków danego ciągu	- len()
- konwersja do stringa - str()
- konwersja na liczbę całkowitą -	int()
- konwersja na liczbę zmiennoprzecinkową	- float()
- przypisanie	 - =
- porównanie	- ==
- wartości logiczne (Boole'an) Prawda/Fałsz -	True / False
### Operatory porównania
- równy	- ==
- nie równy (różny) -	!=
- mniejszy -	<
- większy	 - >
- mniejszy lub równy	- <=
- wiekszy lub równy	- >=
### Operatory logiczne
- i	- and
- lub -	or
- nie -	not
- zawiera - in
- nie zawiera not in
### Kontrola przepływu
- instrukcja warunkowa 'jeśli' -	if
- instrukcja warunkowa 'w przeciwnym razie' -	else
- instrukcja warunkowa 'w przeciwnym razie jeśli -	elif
- pętla 'dopóki' -	while
- instrukcja 'zatrzymaj' -	break
- instrukcja 'kontynuuj' -	continue
- pętla 'dla'	- for
### Funkcje
- definiowanie funkcji	- def nazwa_funkcji():
- definiowanie funkcji z parametrem	- def nazwa(parametr/-y):
- funkcja zwracająca wartość	- def nazwa(): return wartość
- zmienna lokalna w funkcji	- def nazwa(): zmienna
- zmienna globalna poza funkcją -	zmienna = wartość
- zmienna globalna w funkcji	- def nazwa(): global zmienna
- indexowanie zmiennych -	enumerate()
- zakres - range()
- importowanie modułu	- import
- ...

## venv	- Python virtual environment
- pip install virtualenv - zainstalowanie wirtualnego środowiska
- Py -3 -m venv venv - utworzenie środowiska pythona dla danego projektu
- venv/Scripts/activate.bat - aktywacja wirtualnego środowiska Python dla danego projektu
- venv/Scripts/deactivat.bat -	deaktywacja wirtualnego środowiska Python
- venv/Scripts/Activate.ps1 - aktywacja wirtualnego środowiska Python w PowerShellu
- rm -r venv - usuwanie wirtualnego środowiska Pythona
- ...

## PIP - Python Instal Packages
- pip install nazwa_modułu -instalacja wybranego modułu dla danego projektu
- python3 -m pip install nazwa_modułu -jw.
- pip freeze - lista zainstalowanych modułów
- ...

## Python	OOP (Oriented-Objective Programming)
- metoda - funkcja zawarta w klasie i obiektach, które są z niej utworzone
- obiekt - utworzona instancja klasy. Obiekt zawiera wszystkie atrybuty i metody, które zostały zdefiniowane przez klasę. Niektóre dokumentacje obiektowe używają terminu 'instancja' zamiennie z terminem 'obiekt'
- klasa -	szablon, który może być użyty do stworzenie obiektu. Definiuje atrybuty i metody, które będą składały się na obiekt
- klasa bazowa - klasa, która jest rozszerzana, by utworzyć nową klasę pochodną. Klasa bazowa udostępnia klasie pochodnej wszystkie swoje metody i atrybuty
- klasa pochodna -	nowa klasa utworzona w momencie rozszerzenia klasy bazowej. Klasa pochodna dziedziczy wszystkie atrybuty i metody klasy bazowej
- atrybut klasy -	zmienna, która jest częścią klasy
- konstruktor -	opcjonalna, specjalnie nazwana metoda (__init__()), która jest wywoływana w momencie, gdy klasa jest używana do tworzenia obiektu. Zazwyczaj jest ona używana do ustawienia początkowych wartości obiektu.
- destruktor	- opcjonalna, specjalnie nazwana metoda (__del__()), która jest wywoływana w momencie, gdy obiekt jest niszczony. Destruktory są rzdko używane
- dziedziczenie	- tworzenie nowej klasy poprzez rozszerzenie klasy już istniejącej. Klasa pochodna oprócz dodatkwoych atrybutów i metod zdefiniowanych w niej posiada również wszystkie atrybuty i metody klasy bazowej
- ...

## Biblioteki wbudowane
- sring	- operacje na ciągach znaków
- re -operacje na wyrażeniach regularnych
- readline - interfejs GNU readline
- datetime - podstawowe typy daty i czasu
- copy - operacje kopiowania płytkiego i głębokiego
- pprint - drukowanie ładnych danych
- enum - wsparcie dla wyliczeń
- math -	funkcje matematyczne
- random - liczby pseudolosowe
- fractions - liczby wymierne – ułamki
- pathllib - zorientowane obiektowo ścieżki systemu plików
- os.path - manipulacje ścieżkami
- glob - rozszerzanie wzorca ścieżki w stylu UNIX
- shutil - operacje na plikach wysokiego poziomu
- pickle - serializacja obiektów Pythona
- shelve - trwałość obiektow Pythona
- sqlite3 - interfejs DB-API 2.0 dla baz danych SQLite
- csv	- odczytywanie i zapisywanie plików CSV
- os - różne interfejsy systemu operacyjnego
- time - dostęp do czasu i konwersje
- asyncio - asynchorniczne we/wy
- socket - interfejs sieciowy niskiego poziomu
- ssl - opakowanie TLS/SSL dla obiektów gniazd
- email	- pakiet obsługi poczty e-mail i MIME
- json	- koder i dekoder JSON
- html - obsługa HyperTextMarkup Language
- xml	- obsługa XML
- urllib -	moduły obsługi adresów URL
- http - moduły HTTP
- smtplib - klient protokołu SMTP
- tkinter - interfejs Pythona do Tcl/Tk
- unitest - stuktura testów jednostkowych
- venv - tworzenie środowisk wirtualnych
- sys - parametry i funkcje specifyczne dla systemu
- ...

## Biblioteki dodatkowe
- pyperclip - kopiowanie i wstawianie funkcji schowka (clipboard)
- pycurl -	przesyłanie plików poprzez adres URL (obsługuje SSL)
- Beautiful Soup (bs4) -	ułatwia zbieranie danych ze stron internetowych (scrapowanie)
- requests -	prosta biblioteka HTTP
- PyQt5 -	tworzenie interfejsów GUI
- django - framework do tworzenia aplikacji internetowych
- flask -	lekki framework do tworzenie aplikacji internetowych
- jupyter notebook - aplikacja internetowa do tworzenia i udostępniania dokumentów obliczeniowych
- selenium - framework do automatyzacji przeglądarki internetowej
- opencv-python -	framework (cv2) do manipulowania obrazem
- matplotlib -	tworzenie statystyczych, animowanych i interaktywnych wizualizacji
- numpy -	narzędzia do obliczeń naukowych
- pandas - analiza i manipulacja danymi
- ...
