# Strona internetowa szkoły językowej
## Projekt semestralny z przedmiotu Technologie Internetowe
### Informatyka, 3 semestr, Rzeszów 2024

<img src="https://github.com/JustynaToczek/Aplikacja-do-organizacji-czasu/assets/113525212/98861275-57df-4b53-a553-a0576f68ad8e" width="700">

### Spis treści
1. Zdefiniowanie problemu do realizacji</br>
2.	Propozycja rozwiązania problemu</br>
3.	Testowanie</br>
4.	Źródła i prawa autorskie</br>

### 1.	Zdefiniowanie problemu do realizacji
Przygotowany szablon strony reprezentuje stronę szkoły językowej. Odbiorami tej strony powinni być przede wszystkim przyszli klienci prezentowanej szkoły językowej. Strona tworzona jest w celu dobrego zaprezentowania szkoły językowej oraz zachęcenia potencjalnych klientów do skorzystania ze świadczonych usług. Odbiorcy strony internetowej powinni posiadać łatwy dostęp do danych kontaktowych oraz informacji dotyczącej oferty. Strona internetowa powinna pozwolić na przedstawienie świadczonych usług klientowi także w sposób graficzny. Strona internetowa powinna być intuicyjna w użytkowaniu, przejrzysta i posiadać zwięzłe informacje. Strona internetowa powinna otwierać się poprawnie także na urządzeniach mobilnych, bez utraty na swojego wyglądu i responsywności.

### 2.	Propozycja rozwiązania problemu
#### •	Nawigacja
W celu ułatwienia poruszania się po stronie, zastosowane zostało menu główne rozwijane, umieszczone na górze ekranu. Sekcje menu głównego to: Strona główna, Galeria zdjęć, Oferta, Dołącz do nas. Sekcja „Dołącz do nas”, po najechaniu kursorem rozwija się i występuje możliwość wyboru sekcji „Kontakt” lub „Prześlij formularz”. Rozwiązanie rozwijanego menu zostało zastosowane w celu lepszego zorganizowania rozmieszczenia głównych sekcji strony. Efekt menu głównego został uzyskany za pomocą CSS, m.in. dzięki wartościom właściwości display, a rozwijane sekcje dzięki użyciu właściwości position.
#### •	Slider
Na stronie głównej został umieszczony slider zawierający trzy slajdy. Każdy slajd zawiera zdjęcie, jeden z nich przycisk kierujący do oferty szkoły językowej, a dwa pozostałe zawierają napisy. Dzięki użyciu tego rozwiązania zawartość strony lepiej się prezentuje, a jednocześnie w jednym miejscu umieszczone są najważniejsze informacje. Efekt przewijania slidera został uzyskany dzięki znacznikom <a> w HTML, które odsyłają użytkownika we wskazane miejsce (do właściwego slajdu). Efekt wizualny został osiągnięty dzięki regułom CSS. Ogólny wygląd i działanie slidera zostało uzyskane dzięki odpowiednimi wartościami właściwości display, scroll-behavior, overflow-x. Odpowiednie umieszczenie przycisku i napisów na slajdach jest możliwe głównie dzięki wartościom właściwości position.
#### •	Stopka
Na stronie została umieszczona stopka, która zawiera informacje kontaktowe, czyli numer telefonu oraz ikony z przekierowaniem do odpowiednio: twittera, facebooka oraz instagrama. Szablon zawiera mechanizm umiejscowienia stopki zawsze na dole ekranu, bez względu na ilość przedstawianych informacji na stronie. Zostało to uzyskane w CSS, dzięki ustawieniu dla selektora klasy reprezentującego stopkę deklaracji „position: absolute; bottom:0;”, a klasie .container będącej rodzicem klasy stopki ustawienie deklaracji „position: relative”.
#### •	Galeria zdjęć
W sekcji „galeria zdjęć” zostały umieszczone zdjęcia. Są one rozmieszczone w dwóch kolumnach. Efekt ten uzyskano za pomocą CSS dzięki wartości „grid” właściwości „display”.
#### •	Animacje
Strona posiada kilka animacji, które powiększają lub obracają przycisk i obracają obrazy w galerii zdjęć i zmieniają kolor napisów. Animacje użyte są w celu przyciągnięcia uwagi użytkownika i przedstawienia informacji w bardziej ciekawy sposób.
#### •	Zakładki z treścią typu tabs
W sekcji „Oferta” zostały wykorzystane zakładki typu tabs, które po kliknięciu przekierowują użytkownika w odpowiednie miejsce na stronie. Efekt ten został uzyskany dzięki użyciu w kodzie HTML znaczników <a> z atrybutem „href” z przekierowaniem w odpowiednie miejsce.
#### •	Kontener posiadający własny scroll
W tej samej sekcji znajduje się kontener z treścią i tabelami, który posiada własny scroll. Efekt ten został uzyskany dzięki ustawieniu w kodzie CSS dla odpowiedniego elementu wartości „auto” właściwości „overflow”.
#### •	Tabela
W tej samej sekcji znajdują się również dwie tabele stworzone w HTML. Służą one zwięzłej prezentacji danych.
#### •	Mapa
W sekcji „Kontakt” została umieszczona mapa adresu potencjalnie reprezentowanej szkoły językowej. Efekt ten został uzyskany dzięki znacznikowi <iframe> umieszczonemu w kodzie HTML, używanego do osadzenia zasobów zewnętrznych (takich jak np. mapy), z atrybutem „src” zawierającym adres URL docelowej mapy Google. Takie zastosowanie ułatwi użytkownikowi odnalezienie się w aspekcie adresu.
#### •	Formularz
W sekcji „Formularz” został umieszczony formularz, który użytkownik może uzupełnić. Umieszczenie formularza jest użyte w celu interakcji z użytkownikiem. 
#### •	Wyskakujący alert
Podczas wysyłania formularza wykorzystane zostało wyskakujące okienko (alert), stworzone za pomocą operacji DOM. Efekt ten został uzyskany dzięki nadaniu atrybutu „onclick” do przycisku, który przekierowuje do obsługi zdarzenia w JavaScript. W obszarze tej obsługi sprawdzane jest, czy wszystkie wymagane pola formularza zostały wypełnione oraz wykonywana jest walidacja adresu email. 
#### •	Adaptacji treści dla urządzeń mobilnych
Strona internetowa została dostosowana także do urządzeń mobilnych. W celu dostosowania głównego menu do mniejszych ekranów, zostało zastosowane rozwiązanie menu „Hamburger”.

### 3.	Testowanie
#### •	Scenariusz 1 - wypełnianie formularza
##### A.	Użytkownik poprawnie uzupełnia wszystkie pole formularza
Otrzymany rezultat: na stronie wyskakuje okienko z powiadomieniem, że formularz został przesłany. Zrzut ekranu z wyniku testu został przedstawiony na rysunku 1. </br>
<img src="https://github.com/JustynaToczek/Language-school-website/assets/113525212/3517be1c-3259-49ec-8a0f-bc6ceebb937b" width="400"> </br>
Rysunek 1. Realizacja scenariusza 1A
##### B.	Użytkownik pozostawia puste dowolne pole w formularzu.
Otrzymany rezultat: Zostaje wyświetlony alert, informujący użytkownika o niewypełnieniu wszystkich pól formularza. Otrzymany rezultat został przedstawiony na rysunku 2. </br>
<img src="https://github.com/JustynaToczek/Language-school-website/assets/113525212/d2d7c358-8968-4ef4-b644-cfae82864030" width="400"> </br>
Rysunek 2. Realizacja scenariusza 1B
##### C.	Użytkownik wprowadza niepoprawną składnię adresu e-mail.
Otrzymany rezultat: Zostaje wyświetlony alert, informujący użytkownika o niepoprawnie wprowadzonym adresie e-mail. Otrzymany rezultat został przedstawiony na rysunku 3. </br>
<img src="https://github.com/JustynaToczek/Language-school-website/assets/113525212/911869e5-6a10-4cdd-9d78-6c72c5a43ba2" width="400"> </br>
Rysunek 3. Realizacja scenariusza 1C
#### •	Scenariusz 2 – sprawdzanie RWD
##### A.	Użytkownik korzysta ze strony internetowej desktopowo
Oczekiwany rezultat: Zawartość strony wyświetla się prawidłowo, bez żadnych ucięć i utraty treści. </br>
Otrzymany rezultat jest taki sam jak oczekiwany rezultat i został przedstawiony na rysunku 4. </br>
<img src="https://github.com/JustynaToczek/Language-school-website/assets/113525212/50529d5c-6132-4840-ab8b-0c61d62d6f02" width="400"> </br>
Rysunek 4. Realizacja scenariusza 2A
##### B.	Użytkownik korzysta ze strony internetowej na urządzeniu mobilnym
Oczekiwany rezultat: zawartość strony otwiera się w poprawny sposób, dostosowując się do urządzenia mobilnego, bez ucinania treści. </br>
Otrzymany rezultat jest równy oczekiwanemu rezultatowi i został przedstawiony na rysunkach 5 i 6. Treść strony w odpowiedni sposób wyświetla się na różnych urządzeniach mobilnych, nie zatracając przy tym na wyświetlaniu treści. </br>
</br>
<img src="https://github.com/JustynaToczek/Language-school-website/assets/113525212/f8bfe13a-bc7f-4c21-918f-b52002393d3a" width="200"></br>
Rysunek 5. Realizacja scenariusza 2B </br> </br>

<img src="https://github.com/JustynaToczek/Language-school-website/assets/113525212/9a1ef319-c0ed-4d19-a439-ff735d3e7dbc" width="200"> </br>
Rysunek 6. Realizacja scenariusza 2B

### 4.	Źródła i prawa autorskie
Ikony użyte na stronie zostały pobrane ze strony internetowej: https://www.iconfinder.com/ a korzystanie z nich jest dozwolone i darmowe. Zdjęcia użyte na stronie zostały pobrane ze strony internetowej https://pixabay.com/pl/, a dostęp do nich jest dozwolony i darmowy.









