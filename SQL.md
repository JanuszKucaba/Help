# SQL

## Terminologia
- baza danych - plik zorgranizowany tak, by jak najlepiej przechowywać dane
- SQL (Structured Query Language) - ustrukturyzowany język zapytań
- relacja (tabela) - obszar w obrębie bazdy danych, który zawiera krotki i atrybuty (wiersze i kolumny), częściej używa się określenia 'tabela'
- atrybut - jedna z wartości w krotce, częściej nazywany 'kolumną' lub 'polem'
- krotka - pojedyczny wpis w tabeli bazy danych, który jest zbiorem atrybutów, częściej używa się określenia 'wiersz'
- kursor - kursor pozwala na programistyczne wykonywanie poleceń SQL w bazie danych i pobieranie danych z bazy. Kursor jest podobny do gniazda połączeń sieciowych lub uchwytu pliku
- indeks - dodatkowe dane, które oprogramowanie bazy danych przechowuje w postaci wierszy i wstawia dodatkowo do tabeli, dzięki czemu wyszukiwanie informacji odbywa się bardzo szybko
- struktura podstawowa - struktura: tabele (relacja), wiersze (krotka) i kolumny (atrybut)
- tworzenie tabel - tworząc tabelę należy podać nazwę każdej kolumny występującej w tabeli oraz typ danych, który będzie przechowywany w każdej z kolumn – wpływa to na najbardziej efektywy sposób przechowywania i wyszukiwania danych w oparciu o ich typ
- typy danych - zazwyczaj: tekst, liczba lib data
- modelowanie danych - rozbicie danych aplikacji na wiele tabel oraz ustalenie związków pomiędzy nimi
- model danych - dokument projektowy, który pokazuje tabele i ich związki
- klucz logiczny - klucz, którego 'rzeczywisty świat' może użyć do wyszukiwania wierszy, powinienie być unikalny UNIQUE, np. Szukanie po nazwie
- klucz główny - zazwyczaj jest liczbą przypisywaną automatycznie, jest używany tylko do łączenia wierszy z różnych tabel, klucze te są liczbami stałymi, dlatego zajmują bardzo mało miejsca w pamięci i mogą być bardzo szybko porównywane lub sortowane	
- klucz obcy - zazwyczaj jest liczbą wskazującą klucz główny powiązanego wierwsza w innej tabeli
- kiedy zalecane jest używanie bazy danych:
-- gdy aplikacja musi dokonać niewielkiej liczby różnych aktualizacji w ramach dużego zbioru danych,
-- gdy dane są tak duże, że nie mieszczą się w słowniku, a trzeba je wielokrotnie przeszukiwać
-- podczas procesu działającego przez dłuższy czas, który będzie zatrzymywany i uruchamiany ponownie, a jednocześnie należy zachować dane z jednego uruchomienia, tak żeby były dostępne w kolejnym
- normalizacja - projektowanie modelu danych w taki sposób, aby żadne dane nie były powielone. Każdą porcję danych przechowujemy w bazie tylko w jednym miejscu i z innych miejsc odwołujemy się do niej za pomocą klucz obcego.
- ogranczenie - gdy mówimy o bazie danych, by egzekwowała jakąś regułę/zasadę w przypadku kolumny lub wiersza tabeli. Częstym ograniczeniem jest wymuszenie, by w danej kolumnie nie było zduplikowanych wartości (tzn. By wszystkie wartości były unikalne)
- przeglądarka bazy danych - oprogramowanie, które pozwala na bezpośrednie połączenie z bazą danych i zarządzanie nią bez konieczności pisania osobnego programu
- transakcje wg ACID - warunki jakie transakcja (zbiór operacji na bazie danych) musi spełnić: Atomic (niepodzielność), Consistent (spójność), Isolation (odizolowanie), Durability (trwałość)
- ORM Object Relational Mapper, np. SQLAlchemy
- CRUD - Create, Read, Update, Delete

## Zapytania SQL
- CREATE TABLE	- tworzenie tabeli – należy podać dodatkowo nazwy i typy kolumn,	np. CREATE TABLE Utwory (tytuł TEXT, odtworzenie INTEGER);
- INSERT INTO	- wstawianie wiersza do tabeli,	np. INSERT INTO Utwory (tytuł, odtworzenia) VALUES ('My Way', 15);
- SELECT * INTO	- wyświetlanie całej zawartości danej tabeli, np. SELECT * INTO Nazwa bazy;
- SELECT DISTINCT	- wyświetla pojedyncze wpisy danej kolumny, np. SELECT DISTINCT Country FROM Customers;
- SELECT COUNT(DISTINCT) -	wyświetla ilość wierszy, np. SELECT COUNT(DISTINCT Country) FROM Customers
- SELECT {co} FROM {skąd} ORDER BY {sort} LIMIT {ile wydać} OFFSET {ile przeskoczyć}		
- SELECT COUNT(kol) FROM {skąd} GROUP BY {kol} - agregowanie danych
- SELECT kolumna INTO
- SELECT * FROM Tabela -	wyświetla zawartość całej tabeli
- SELECT Kol1, Kol2 FROM Tabela	- wyświetla zawartość danych kolumn w tabeli
- ORDER BY Kol - sortowanie wyników	SELECT Kol1, Kol2 FROM Lista ORDER BY Kol1
- WHERE	- Odfiltrowuje dane zależne od warunku, np.	SELECT * FROM Tabela WHERE kolumna = warunek
- WHERE AND OR	- warunki logiczne i/oraz, lub, np. SELECT * FROM Tabela WHERE kol1 = 1 OR kol2 = 'TAK' AND kol3 = 1
- WHERE IN - porównuje kolumnę z wieloma możliwościami, zwraca True albo False, np. SELECT * FROM Tabel WHERE kol1 IN (2, 3)
- WHERE BETWEEN	- Kolumna o zadanym zakresie, np.	SELECT * FROM Tabela WHERE kol1 BETWEEN x AND y
- WHERE LIKE	- Elementy o nazwie wg wzoru, np. SELECT * FROM Tabela WHERE kol1 Like 'Nazwa'
- COUNT() -	zlicza liczbę wierszy, np.	SELECT COUNT(*) FROM Tabela
- SUM() -	zwraca całkowitą sumę wartości w danej kolumnie liczbowe
- AVG() -	zwraca średnią z wartości
- MIN() / MAX()	- zwraca najmniejszą / największą wartość, np. SELECT MAX(Kol1) FROM Tabela
- SELECT Kol1, Kol2 FROM Tabela WHERE Kol3 = (SELECT MIN(Kol3) FROM Tabela)	- zagnieżdzanie
- INSERT	INSERT
- DELETE - usuwanie wiersza, np.	DELETE FROM Utwory WHERE tytuł = 'My Way'
- DROP TABLE	DROP TABLE
- UPDATE - aktualizacja kolumn, np. UPDATE utwory SET odtworzenia = 16 WHERE tytuł – 'My Way'
-	Sqlite.connect('nazwa_bazy') – połączenie z BD, *.cursor – otwarcie BD, *.execute – wykonanie polecenia na bazie commit() - zapis danych do pliku
- SELECT - sortowanie, np. SELECT tytuł, xxx FROM aaaa ORDER BY tytuł