# ProjektKoncowy - Zarządzanie koszykiem na stronie komputronik.pl

## Spis treści
* [Opis projektu](#opis-projektu)
* [Technologie](#technologie)
* [Analiza ryzyk - przykłady](#Analiza-ryzyk---przykłady)
* [Przypadki testowe w narzędziu TestRail - przykłady](#Przypadki-testowe-w-narzędziu-TestRail---przykłady)
* [Przypadki testowe w metodyce Behavior Driven Development (BDD)](#Przypadki-testowe-w-metodyce-Behavior-Driven-Development-(BDD))
* [Karty sesji eksploracyjnej - przykłady](#Karty-sesji-eksploracyjnej---przykłady)
* [Raportowanie defektów w narzędziu JIRA - przykłady](#Raportowanie-defektów-w-narzędziu-JIRA---przykłady)
* [Nagrywanie testów za pomocą narzędzia Selenium IDE](#Nagrywanie-testów-za-pomocą-narzędzia-Selenium-IDE)
* [Korzystanie z narzędzi deweloperskich w przeglądarce internetowej](#Korzystanie-z-narzędzi-deweloperskich-w-przeglądarce-internetowej)
* [Wysyłanie requestów za pomocą narzędzia Postman](#Wysyłanie-requestów-za-pomocą-narzędzia-Postman)

## Opis projektu

Przeprowadzenie procesu testowego obejmującego: 
- analizę wymagań oraz ryzyk
- opracowanie test planu
- opracowanie oraz wykonanie przypadków testowych obejmujących testy funkcjonalne, niefunkcjonalne oraz sesje eksploracyjne, również w metodyce BDD.
- raportowanie defektów
- opracowanie raportu końcowego

Strona internetowa z obszaru e-commerce ma umożliwić użytkownikowi dodawanie produktów do
koszyka, edytowanie jego zawartości oraz przechodzenie do etapu finalizacji zamówienia.

## Technologie

- TestRail
- JIRA
- Confluence
- Postman
- Selenium IDE
- DevTools w Google Chrome

## Analiza ryzyk - przykłady

 Ryzyka produktowe | Plan złagodzenia
 --- | ---
 Wysoka złożoność struktury modułu | Wzajemne wsaprcie zespołu
 Duże zależności między systemami: zespół z Polski tworzy frontendm a za warstwę backend'ową odpowiada firma zewnętrzna ze Skandynawii | Zadbanie o dobrą komunikację między zespołami
Stosowanie innowacyjnej architektury tworzenia oprogramowania | Najbadziej złożonymi częściami tworzonego oprogramowania zajmować się będą najlepiej przeszkoleni i doświadczeni deweloperzy
napięte harmonogramy | Zadbanie o opdpowiednią estymację czasu pracy zespołu

Ryzyka projektowe | Plan złagodzenia
--- | ---
Niewystarczające kwalifikacje zespołu testerskiego | Wsparcie Test Managera oraz przeprowadzenie dodatkoych szkoleń
Braki kadrowe | Wsparcie testerów z innych zespołów
Niska jakość artefaktów testowych | Wsparcie Test Managera na każdym etapie procesu testowego i zadbanie o wysoką jakość tworzonych artefaktów
Błędy lub braki w dokumentacji | od początku procesu testowego szczegółowa analiza wymagań oraz dokumentacji
Niedziałąjące lub niedostępny środowisko testowe | Zadbanie o dostęp do środowiska testowego oraz wzajemne wsparcie zespołu
Niedostępne narzędzia | Zadbanie o dostęp do narzędzi poprzez wykupienie odpowiednich licencji
Problemy w komunikacji w zespole | Częste spotkani w zespole i integracja jej członków
Brak wsparcia kadry zarządzającej | Szkolenia menedżerskie dla kadry zarządzającej oraz motywowanie jej do wspierania zespołu
Bariery językowe | Kursy językowe lub wsparcie lektora
Niski standard pracy w metodyce Scrum | Szkolenia dla zespołu ze sposobu wytwarzania oprogramowania w sposób zwinny, w metodyce Agile (framework - Scrum)

## Przypadki testowe w narzędziu TestRail - przykłady
![Zrzut ekranu 2023-02-27 o 23 12 15](https://user-images.githubusercontent.com/116351258/227199057-8059d1bb-c9ac-490a-9565-8dec55944d2e.png)
![Zrzut ekranu 2023-02-27 o 23 14 51](https://user-images.githubusercontent.com/116351258/227199112-b3279d63-50de-40aa-8ca8-4bda3e9d829b.png)

## Przypadki testowe w metodyce Behavior Driven Development (BDD)
![Zrzut ekranu 2023-02-27 o 23 38 55](https://user-images.githubusercontent.com/116351258/227204307-ec616538-9607-41a8-beda-efd9ccfb52dd.png)

## Karty sesji eksploracyjnej - przykłady
![Zrzut ekranu 2023-03-23 o 13 10 58](https://user-images.githubusercontent.com/116351258/227200043-b5a3896c-ce96-4cd4-82fc-4bce65db99ec.png)
![Zrzut ekranu 2023-03-23 o 13 11 12](https://user-images.githubusercontent.com/116351258/227200098-ecedea67-9637-4271-b4b6-58b70a101271.png)
![Zrzut ekranu 2023-03-23 o 13 11 23](https://user-images.githubusercontent.com/116351258/227200151-40e910d8-5f4e-4aa2-8215-66e714b82d5e.png)

## Raportowanie defektów w narzędziu JIRA - przykłady
![Zrzut ekranu 2023-03-23 o 13 18 13](https://user-images.githubusercontent.com/116351258/227201800-8fe9e337-9e33-40f0-9aee-899e4e86ee3d.png)
![Zrzut ekranu 2023-03-23 o 13 18 57](https://user-images.githubusercontent.com/116351258/227201833-ef0fa5ef-a420-4140-a843-cbfcba79f954.png)

## Nagrywanie testów za pomocą narzędzia Selenium IDE
![Zrzut ekranu 2023-02-27 o 23 28 50](https://user-images.githubusercontent.com/116351258/227202168-e99f8984-e05b-4c11-bbc4-6f9c1c892494.png)

## Korzystanie z narzędzi deweloperskich w przeglądarce internetowej
- Ilość niewykorzystanych bajtów w załadowanych plikach
![Zrzut ekranu 2023-02-25 o 15 53 28](https://user-images.githubusercontent.com/116351258/227202728-15028679-c0af-4f2f-8424-9c1f5c7bcfe7.png)

- Identyfikacja elementów na stronie wraz z zastoaowanym stylem
![Zrzut ekranu 2023-02-27 o 23 46 54](https://user-images.githubusercontent.com/116351258/227202958-3f9824fb-3f36-4cb4-9c9a-815aa9b0e404.png)

- Audyt

![Zrzut ekranu 2023-03-23 o 13 28 15](https://user-images.githubusercontent.com/116351258/227204007-f1fec9b5-4237-4f0c-aa6f-d183b85ee9f3.png)

## Wysyłanie requestów za pomocą narzędzia Postman
- metoda GET
![GET](https://user-images.githubusercontent.com/116351258/227205117-f0895dea-fcc6-4ed1-a72a-a4747825cefe.png)
- metoda POST
![POST](https://user-images.githubusercontent.com/116351258/227205209-0f9d8275-b303-443a-8dc2-dc239b42a814.png)
- metoda PUT
![PUT](https://user-images.githubusercontent.com/116351258/227205276-978b7ffe-e231-4bfa-99cc-43ed4923309c.png)
- metoda DELETE
![DELETE](https://user-images.githubusercontent.com/116351258/227205338-563efcdc-d992-4db2-aa98-66f5833ffe28.png)






