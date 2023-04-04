# Przypadki testowe opracowane w narzędziu do zarządzania przypadkami testowymi TestRail

![testrail](https://user-images.githubusercontent.com/116351258/229790414-60beb537-74da-4c21-97e5-7e0ff3a3686e.png)

TestRail to elastyczne narzędzie do zarządzania przypadkami testowymi z intuicyjnym interfejsem użytkownika. Umożliwia łatwe tworzenie, łączenie i ponowne wykorzystywanie przypadków testowych i grupowanie ich w zorganizowanej strukturze. Dodatkowo pozwala śledzić wyniki testów w czasie rzeczywistym i generuje szczegółowe raporty na temat testów, obciążenia zespołu, pokrycia kodu i innych.

Narzędzie składa się z kilku sekcji:

**Overview** — jest to sekcja, w której widzimy aktualny stan naszego projektu. Widzimy aktualne wyniki testów, kamienie milowe, aktywność użytkowników oraz rzeczy do wykonania.

**TODO** — zadania do wykonania, które można przypisać poszczególnym użytkownikom.

**Milestones** — kamienie milowe, czyli kluczowe etapy projektu do osiągnięcia. Kamienie milowe mogą być powiązane z wykonaniem określonych przypadków testowych. Pokrycie kamieni milowych w takim przypadku mierzy się w procentach.

**Test Runs & Results** — miejsce, w którym tworzy się zbiory przypadków testowych (Test Run), a następnie dokonuje ich egzekucji. Wyniki testów należy zaktualizować ręcznie lub przy pomocy zapytania Rest API. Do wyników testów można i zaleca się dołączać zrzuty ekranu czy logi z wykonania testu.

**Test Cases** — sekcja, w której tworzy się przypadki testowe. Narzędzie Test Rail wspiera kilka formatów tworzenia przypadków testowych: format tekstowy, sesja eksploracyjna. Celem utrzymania porządku przypadki testowe można umieszczać w poszczególnych sekcjach. Narzędzie umożliwia wyszukiwanie oraz sortowanie przypadków testowych w zależności od zadanych kryteriów.

Dobry przypadek testowy powinien posiadać wszystkie wymagane informacje. Zaczynając od dobrego 

👉**tytułu**, który pozwoli na skojarzenie przypadku testowego z planowanym działaniem testowym, lub testowanym komponentem. 

Pozostałymi ważnymi informacjami, które należy uzupełnić są: 

👉 **Sekcja (Section)** - czyli folder, do którego chcielibyśmy przyporządkować przypadek testowy. 

👉 **Wzorzec (Template)** - czyli sposób opisania kroków do wykonania. Test Rail oferuje trzy możliwości, najbardziej popularnym rozwiązaniem jest rozbicie działań na kroki do wykonania i oczekiwane rezultaty. 

👉 **Typ Testu (Type)** - wybór testu pozwala uporządkować repozytorium testowe, grupując przypadki testowe np. na przypadki testowe funkcjonalne/niefunkcjonalne. 

👉 **Priorytet (Priority)** - czyli nieformalna kolejność wykonywania przypadków testowych. Im wyższy priorytet, tym szybciej powinien wykonany być test. W przypadku ograniczonej ilości czasu, na podstawie analizy ryzyka można pominąć przypadki testowe o niskim priorytecie lub wykonać je jako ostatnie. 

👉 **Estymacja (Estimate)** - czas potrzebny na wykonanie danego przypadku testowego. * Referencje, odniesienia do dokumentów (References) - w tym miejscu możesz umieścić informacje o identyfikatorze dokumentu lub wymagania, na podstawie którego został utworzony przypadek testowy. 

👉 **Typ Automatyzacji (Automation Type)** - Test Rail wspiera automatyzacje testów w narzędziu Ranorex. Pole to nie jest obowiązkowe do wypełnienia. 

👉 **Warunki Wstępne (Preconditions)** - wszelkie działania, wymagane oprogramowanie, które będzie potrzebne do wykonania przypadku testowego.
