# Różnoraka wiedza z IT
1. Terminologia
2. Chmura AWS
3. RESTful API
4. Linux

## 1. Terminologia
- CI -	Continuous Integration
- CD -	Continuous Delivery
- TDD	- Test-Driven Development -	technika tworzenie oprogramowanai poprzez pisanie testów automatycznych przed napisaniem danej funkcjonalności
- DDD	- Domain-Driven Design - tworzenie oporogramowania poprzez definiowanie obiektów i komponentów systemu oraz ich zachowań, tak aby wiernie odzwierciedlały rzeczywistość
- BDD	- Behavior-Driven Development	- połączenie TDD z DDD i OOAD (obiektowo-zorientowanej analizy  i projektowania
- DevOps - Developer Operations
- Refaktoring	- proces wprowadzania zmian w projekcie/programie, w wyniku których zasadniczo nie zmienia się funkcjonalność
- API	- Application Program Interfaces - interfejsy programowania aplikacji	- umowa pomiędzy aplikacjami, która określa schematy interakcji pomiędzy dwoam komponentami tych aplikacji
- JSON - notacja obiektowa JavaScript	- format, który pozwala na oznakowanei ustrukturyzowanych danych w oparciu o składnię  obiektów JavaScript
- XML - rozszerzalny język znaczników	- format, który pozwala na oznakowanei danych strukturalnych
- SOA	- Service-Oriented Architecture	- architektura usługowa - sytuacja w której aplikacja składa się z połączonych w sieci komponentów	podejście SOA oznacza, że cała nasza aplikacja korzysta z usług innych aplikacji, np rezerwacja samochodu albo hotelu z poziomu strony linii lotniczej	
- web service - usługa sieciowa	

## 2. CHMURA AWS
- AWS	- Amazon Web Services
- FaS	- Function as Service -	kod źródłowy w chmurze np. Lambda
- IaC -	Infrastructure as Code - tworzenie wirtualnych elementów sieci na chmurze przy pomocy kody – tworzenie kody bez tworzenia aplikacji
- AWS Lambda - serwer do Pythona w chmurze	Ty podajesz swój kod źródłowy, a AWS automatycznie tworzy serwer, wykonuje Twój kod, zwraca Ci wynik i usuwa serwer. A wszystko jest możliwe w czasie dużo ponizej 1 sekundy.
- AWS Fargate -	tworzysz obrazy kontenerowe, a Fargate automatycznie tworzy za Ciebie kontenery oraz całą infrastrukturę (serwery, load balancery a nawet VPC) i uruchamia Twoją aplikację. Znowu - oprócz stworzenia obrazu kontenerowego z Twoją aplikacją, nie musisz zajmować się niczym więcej.	
- CloudWatch -zbiera logi na repozytorium, ale są kasowane po wykasowaniu serwera
- AutoScaling	- tworzenie i kasowanie się serwerów w zależności od ruchu na stronie – dynamicznie
- EFS - Elastic File System -	share drive na którym można zapisać logi
- Boto3 - biblioteka Pythona do zarządzania AWS – tworzenie infrastruktury
- CDK	- Cloud Development Kit - do tworzenie bardzo dużych i skomplikowanych infrastruktur i konfigurowania ich między sobą
- Serwer Django -	gotowy serwer Python Django
- S3 - serwer np. Na pliki

## 3. RESTful API
- REST - REpresentational State Transfer
- interfejsy są oparte o zasoby
- każdy zasób ma swój identyfikator URI
- interakcja z usługą odbywa się przez wymianę ustandaryzowanej reprezentacji zasobów, np. notacji JSON, XML
- interfejsy są ustandaryzowane , każda metoda służy do zrobienia jednej operacji, wywołanie na danym zasobie np. GET spowoduje zwrócenie zasobu, a PUT aktualizację jego wartości
- żądania są bezstanowe, do zrozumienia odpowiedzi nie jest potrzebna wiedza o poprzednim żądaniu
- połączenia w odpowiedzi są reprezentowane przez hiperłącza.

## 4. Linux
- ls - listing plików w danym folderze
- cd - poruszanie się po folderach
- su - przelogowanie się na innego użytkownika
- source - uruchamia plik w obecnej powłoce (konsoli)
