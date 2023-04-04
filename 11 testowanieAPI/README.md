# Testowanie API w POSTMAN

![image](https://user-images.githubusercontent.com/116351258/229900923-418f1965-35cc-4fa4-8881-f267c44f143c.png)

Narzędzie Postman może być świetnym narzędziem to testowania warstwy back-endowej naszej aplikacji (czyli API). Narzędzie to ze względu na swoje możliwośći pozwala nie tylko na wysyłanie żądań (i co za tym idzie) i manualna weryfikacje ale także tworzenie testów automatycznych za pomocą wbudowanych snippetów kodu Java-Script.

## POSTMAN
**Postman** jest bezpłatnym narzędziem, które możemy wykorzystać do testów API. Narzędzie nie wymaga instalacji i może być zainstalowane jako dodatek do przeglądarki Google Chrome, oczywiście to tylko jedna z możliwości, osoby zainteresowane mogą zainstalować narzędzie na swoim własnym komputerze (wsparcie dla Windows, Linux oraz Mac).

Postman służy głównie do wysyłania żądań różnego typu:
* GET
* POST
* PUT
* DELETE

Są to cztery najbardziej popularne żądania wysyłane przy pomocy REST API. Więcej informacji na temat metod http można przeczytać w [Dokumentacji](https://developer.mozilla.org/en-US/docs/Web/HTTP/Methods)

Po każdym z wysłanych żądań, wysyłany jest kod odpowiedzi w postaci trzycyfrowego numeru. Pierwsza liczba kodu odpowiedzi definiuje rodzaj komunikatu. Są to odpowiednio:
* Kody informacyjne - rozpoczynające się od 1, np. 101, 111
* Kody powodzenia - rozpoczynające się od 2, np. 200, 201
* Kody przekierowania - rozpoczynające się od 3, np. 301, 306
* Kody błędu aplikacji klienta - rozpoczynające się od 4, np. 404
* Kody błędu serwera HTTP - rozpoczynające się od 5, np. 500, 501

Każdy kod odpowiedzi posiada swoją reprezentację opisową. Pełną listę kodów odpowiedzi http można zobaczyć tutaj

### Kolekcje
Żądania w narzędziu Postman są grupowane w kolekcje. Kolekcje stanowią folder z żądaniami, które będziemy wysyłać za pomocą narzędzia, mogą to być zapytania różnego typu. Kolekcję można eksportować do pliku, co umożliwia wersjonowanie lub zaimportować na podstawie pliku wejściowego, lub wpisać własnoręcznie ciąg znaków.

### Żądania - Requests
Wysłanie żądania odbywa się poprzez wybór rodzaju żądania i wpisanie adresu, na który będziemy wysyłać nasze żądanie. Adres końcowy (ang. endpoint) to adres naszej usługi sieciowej. Do usługi sieciowej zapytanie może zostać wysłane z konkretnymi parametrami, które są wysyłane w formacie klucz:wartość, każdy parametr musi być oddzielony znakiem &.
Każde żądanie musi spełnić warunki autentykacji, czyli logowania do usługi sieciowej. Pewne usługi są dostępne tylko dla zalogowanych użytkowników, podobnie jak dostęp do naszej skrzynki mailowej uzyskujemy dopiero po poprawnym zalogowaniu się. Postman oferuje kilka rodzajów autentykacji użytkownika.

### Autoryzacja - Authorization
Autoryzacja jest mechanizmem, który ma na celu zweryfikować, że dany użytkownik ma dostęp do zasobów konkretnego API. Innymi słowy, mówiąc, czy może się zalogować. W serwerze, do którego będziemy wysyłać żądania może istnieć wielu użytkowników lub dostępy do niektórych zasobów mogą być ograniczone.

### Parametry
Istnieją dwie podstawowe metody przekazania parametrów:
* jako element URL przy użyciu metody GET
* jako treść elementu ciała (body) żądania przy użyciu metody POST

Parametry przekazywane metodą GET umieszczane są w adresie strony po znaku `?` i rozdzielone znakiem `&`. Parametry są zwykle przekazywane w postaci par nazwa=wartość.

Przykład:
`https://www.google.pl/search?q=get+method+example&lr=lang_pl`

### Nagłówki
Nagłówki HTTP spotkamy zarówno w zapytaniach, jak i w odpowiedziach. Są one pierwszymi liniami, oddzielone od ciała jedną pustą linią. Nagłówki są opcjonalne – protokół nie wymaga ich obecności. Nagłówki to pewnego rodzaju metadane i polecenia wymieniane przez przeglądarkę i serwer – mogą się w nich znaleźć informacje takie jak rodzaj przesyłanych treści (np. czy jest to obrazek, czy plik JSON), sugestia dotycząca traktowania zawartości (czy przeglądarka ma wyświetlić daną treść, czy np. potraktować to jako pobieranie), jaki jest rozmiar przesyłanych danych, kiedy były modyfikowane, jakiego rodzaju odpowiedzi druga strona się spodziewa itp.

### Ciało - body
Ciało wiadomości przechowuje rzeczywiste dane żądania HTTP (takie jak dane formularza, etc.) i dane odpowiedzi HTTP z serwera ( pliki, obrazki, JSON, etc.). Wyróżnia się kilka rodzajów Body. Wszystko zależy od tego, na jaką formę zezwala punkt końcowy, do którego wysyłamy żądanie.

## Odpowiedź
Odpowiedź jest to informacja z serwera o tym, czy nasze żądanie skończyło się poprawnie. Informacje otrzymujemy w postaci kodu odpowiedzi http oraz w zależności od tego, co zwraca serwer ciało, odpowiedzi w formacie json, xml, html lub formacie tekstowym.

## Testy - Tests
Wszystkie żądania, które były dotychczas przez Ciebie tworzone musiały być zweryfikowane przez Ciebie ręcznie. Czy status odpowiedzi się zgadza? Czy odpowiedź przyszła w założonym czasie? Czy ciało odpowiedzi zawiera określone wyrażenia? To tylko kilka przykładów testów, które musisz wykonywać po wykonaniu każdego żądania. Gdy liczba stworzonych requestów wzrasta, trzeba na to poświęcić coraz więcej czasu. Z pomocą przychodzi nam zakładka tests oraz gotowe do wykorzystania przykłady (snippety).

Testy są wykonywane w tym samym momencie co żądanie, jego wynik obserwujemy pod kodem. Wyniki można filtrować w celu odnalezienia interesujących nas statusów.

## Code Snippet
Pomimo szerokich możliwości narzędzia Postman co do tworzenia żądań oraz pisania prostych testów. Utrzymywanie kolekcji nie jest sprawą prostą, ponieważ same kolekcje są zapisywane w pliku JSON, który w przypadku zaawansowanych kolekcji żądań może mieć długość do kilkuset tysięcy linijek!. Testy przygotowane w aplikacji Postman można automatyzować przy pomocy wybranego języka programowania. Postman ma specjalną funkcję code snippet, która umożliwia eksport żądania do kodu źródłowego w wybranym języku programowania. Przez co późniejsza automatyzacja testów staję się prostsza.

## Runner
Runner jest to specjalna funkcja aplikacji Postman, która pozwala na uruchomienie więcej niż jednego zapytania jednocześnie np. całej wybranej kolekcji. Po wykonaniu zestawu zapytań narzędzie wyświetla podsumowanie: ilość poprawnie wykonanych żądań, ilość niepoprawnych żądań, czas trwania. Każde kolejne uruchomienie tego samego zestawu żądań, powoduje zarchiwizowanie poprzednich wyników, dzięki czemu istnieje możliwość porównania wyników testów, na różnych wersjach aplikacji.
