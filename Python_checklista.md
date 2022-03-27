# Checklista Python

### Minimalna wiedza
1. If – instrukcje warunkowe	else, elif, co True, co False, <, > equal
2.	zmienne	czym się == vs =
3.	typy	int, float, str, dynamiczne typowanie,
4.	listy	Lista = [], lista.append(). Lista.extend(). Lista.index(), lista.pop()
5.	tuple	Tupla = (1, 2, 3), t[1] # 2, t.index(1) # 0, t.count(3) # 2, zawsze używaj tupli zamiast listy jak się da
6.	Set-y	trzyma tylko obiekty, które są unikalne, s = {1, 1,1, 1, 1} # jedynka i tak będzie tylko raz
7.	Dict-y słowniki	Slownik = {1: 'a', 2: 'b'}, for key, value in slownik.items(): pass, jak wygląda dostęp, po co są klucze, jak się iterować po kluczach, wartościach, wartościach i kluczach, bardzo szybki, hashing, hashowanie słownika
8.	for	for element in [1, 2, 3]: print(x)
9.	zip	for x, y in zip([1, 2, 3], [4, 5, 6]): print(x) # 1; print(y) # 4, różne długości list
10.	all i any	all([True, True, True]) # True; all([True, True, False]) # False; any([False, False, False]) # False; any([False, False, False]) # True, any all na pustę kolekcji
11.	range	for x in range(1, 10): print(x), jak się używa, do czego służy, jak wystartować nie od zera itp.
12.	fstring	X = 10; print(f'x = {x}')
13.	Slice-ing	Lista = [1, 2, 3, 4], nowa_lista = lista[1:2] # [2], co to jest, zakresy, czy modyfikuje, czy zwraca nową
14.	funkcje	co to jest funkcja, parametry, return, a jak nie ma, jak przekazać funkcje jako parametr do drugiej
15.	args i kwargs	def func(*args, **kwargs): pass – przyjmowanie wszystkiego
16.	mutable i immutable (zmienne i niezmienne)	tupla jest niezmienna, listę można modyfikować co to znaczy, jaki ma to wpływ na program i jak jest ze strigniem, tupla = (1, 2, 3), tupla[0] = 3 # exception
17.	tuple unpacking (rozpakowywanie tupli)	x, y  = (1 ,2)
18.	shallow copy and deep copy	Lista = (1, {'a':2}, 3); nowa_lista = lista[:], które kopiowanie jest lepsze i czym od siebie się różnią
19.	list comprehension	listy składane [x for x in range(10)]
20.	dict comprehension	{x: x for x in range(10)}
21.	set comprehension	{x for x in range(10)}
22.	generatory	do czego służa, jaki problem generują, czemu oszdzędza pamięć, jak go napisać, do czego jest yield, czy jeden generator może wywołać drugi generator
23.	dekorator	do czego służą, kiedy się ich używa, jak napisać dekorator @, po co się je pisze, jak napisać własny, kiedy można go użyć
24.	OOP	tworzenie obiektów, jak się tworzy klasy, po co się tworzy klasy, co nam to upraszcza, czym się różni instancja od obiektu, do czego służy metoda init
25.	wszystko jest obiektem	
26.	dziedziczenie	po co jest dziedziczenie, co to znaczy że jedna dziedziczy po drugiej, jaki problemy rozwiązuje, do czego to się używa, przed czym nas to chroni
27.	zmienne statyczne	
28.	metody statyczne	
29.	metody abstrakcyjne	
30.	kompozycja, a dziedziczenie oraz agregacja	
31.	magic methods	
32.	rekurencja	wywołanie funkcji wewnątrz funkcji, 
33.	context manager	
34.	exceptions	
35.	JSON	co to jest, do czego służy, jak to się ma do dicta,
36.	namedtuple	jaki problem rozwiazuje, czy można się iterować jak po tuply
37.	dataclasses	generator kodu
38.	Multithreading, asyncIO	
39.	lambda	do czego służy, jak używać z filter i map
40.	iterable iterator	
41.	import	import modułów, w jakiej kolejności, czemu nie importować z *
42.	PIP	packet installer for python, jak używać, co znaczy -r, jak sprawdzać wersję
43.	pliki	jak czytać
44.	type annotations	
45.	property	dlaczego nie trzeba robić settterów i getterów
46.	pep8	
47.	enumerate	jak go używać, jak wystartować nie od 0
48.	itertools	poczytać dokumentację
49.	testy jednostkowe	pytest, co to jest, do czego służy
50.	regex	regular expressions
51.	virtual enviroment	
52.	linting	pylint
53.	assignment expression	Od 3.8 if (n := len(a)) > 10: pass
54.	structural pattern matching (od 3.10)	Match / case (tak jak switch/case)
55.	przekazywanie argumentów do funkcji (metod)	
56.	wyrażenia generatorowe	
57.	multiprocessing	
58.	python turtle
59.	Big O notation
