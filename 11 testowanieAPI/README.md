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

Parametry przekazywane metodą GET umieszczane są w adresie strony po znaku ? i rozdzielone znakiem &. Parametry są zwykle przekazywane w postaci par nazwa=wartość.

Przykład:
'https://www.google.pl/search?q=get+method+example&lr=lang_pl'
