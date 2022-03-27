#Notes
git config --global user.name "nazwisko" - zmiana nazwiska globalnie
git config --global user.email "mail@domena.pl" - zmiana maila globalnie
git congif user.name "nazwisko" - zmiana nazwiska dla danego repozytorium
git config user.email "mail@domena.pl" - zmiana maila dla danego repozytorium
git init    - tworzy nowe repozytorium w istniejącym projekcie
git clone   - pobiera repozytorium zdalne
donwload ZIP na githubie - pobiera pliki odłaczając je od git-a
git status  - sprawdza stan repozytorium
git add     - dodajemy plik do śledzenia
git add nazwa pliku - dodaje dany plik do śledzenia
git add nazwa . - dodajemy wszystkie pliki w wybranym folderze do śledzenia
git rm -- cached nazwa pliku - usunięcie pliku ze śledzenia
git reset   - usunięcie wszystkich plików ze śledzenia
git commit  - wysłanie zmiany do lokalnego repozytorium z komentarzem
ctrl-x + ctrl-c + :wq         - kończenie zapisu commit w konsoli vi
git restore nazwa pliku - przywrócenie pliku do wersji z repozytorium
git commit --author="nazwisko <mail@domena.pl>" - zmiana nazwiska i maila dla kolejnego commita
git log     - wyświetlenie wszystkich commitów, któr wykonaliśmy w repozytorium
git revert nr_hash  - cofnięcie określonego commita
git show nr_hash    - wyświetlenie informacji o konkretnym commicie
git clone adres_repo - kopiowanie repozytorium z githuba
git push    - publikuje lokalne zmiany (wysyłam je do repozytorium zdalnego)
git pull    - pobieram zmiany ze zdalnego repozytorium
git checkout -b NazwaBranchu - utworzenie nowej gałęzi
git commit -m 'komentarz' - wysłanie zmiany z komentarzem do lokalnego repo