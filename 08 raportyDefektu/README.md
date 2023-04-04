# Raporty defektu w narzędziu JIRA poprzez TestRail'a (integracja)

![image](https://user-images.githubusercontent.com/116351258/229881315-7400e5c2-95ed-4ba5-95fd-0a5266636d92.png)


**JIRA** — według definicji jest to zamknięte oprogramowanie do śledzenia błędów oraz zarządzania projektami. W praktyce jednak jest to platforma do organizowania pracy zespołów w dużych organizacjach, rozproszonych globalnie. Jest to narzędzie niezwykle intuicyjne i zawierające szerokie możliwości konfiguracji oraz integracji z bardzo dużą ilością narzędzi dostępnych na rynku. Składa się z trzech głównych komponentów:

**Jira Core** – podstawowa platforma, system do zarządzania pracą zespołu.

**Jira Software** – tworzenie tablic SCRUM oraz Kanban, tworzenie raportów dla zespołów Agile'owych. Integracja z narzędziami deweloperskimi (narzędzia do wersjonowania kodu, narzędzia do zarządzania testami). Głównie stosowana przez zespoły deweloperskie.

**Jira Service Desk** – dedykowana dla zespołów, które na co dzień obsługują zgłoszenia klientów wewnętrznych lub zewnętrznych z możliwością mierzenia i raportowania SLA (ang. Service Level Agreement).

## Tablice w JIRA
Narzędzie JIRA wspomaga śledzenie pracy zespołu przy pomocy tablic. Wyróżnia się ich trzy rodzaje:

**Tablica Scrum** pomaga zespołom w zarządzaniu historiami, zadaniami i błędami w pojedynczych sprintach w określonych ramach czasowych. Tablice Scrum są najbardziej odpowiednie dla tych zespołów, które pracują nad dużymi projektami.

**Tablice Kanban** pomagają zarządzać historiami, zadaniami i błędami w ciągłym przepływie pracy. Dobrze sprawdzą się w przypadku zespołów, które muszą mieć większą kontrolę nad ilością pracy w backlogu.

**Tablice Agility** to tablice do zarządzania zadaniami przy pomocy elastycznego i prostego w obsłudze interfejsu. Są doskonałym wyborem dla zespołów, które nie mają dużego doświadczenia w metodyce agile lub nie chcą poświęcać zbyt wiele czasu na indywidualne konfigurowanie przepływu pracy.

## Rodzaje zgłoszeń w JIRA
Podstawowymi rodzajami zgłoszeń w JIRA są: epiki (duże zestawy historyjek użytkownika), story (pojedyncze historyjki użytkownika), defekty (defekty zgłoszone przez testerów lub innych uczestników projektu), taski (czyli wszystkie inne zadania). Każde ze zgłoszeń wyróżnia się pewnymi charakterystycznymi elementami, część elementów pozostaje natomiast wspólna: tytuł, opis zgłoszenia, labelki, ilość zaplanowanego czasu czy sprint, w którym dane zadanie należy wykonać. Dzięki dużym możliwościom konfiguracyjnym JIRY administrator projektu może samodzielnie zdefiniować pola lub sprawić, że pewne pola będą obowiązkowe np. kroki do reprodukcji w przypadku defektu.

## Wyszukiwanie zgłoszeń w JIRA
W Jira mamy dwa typy wyszukiwania. Pierwszy to basic, który pozwala filtrować zgłoszenia po kryteriach uzupełnianych w sposób graficzny (wybieranie wartości z pól).

Drugim sposobem jest stworzony przez Atlassiana JQL – JIRA Query Language. Bardzo elastyczny i dostarczający wiele opcji sposób wyszukiwania. Nie trzeba znać JQL na pamięć, w sieci jest dostępnych wiele tutoriali oraz ściągawek np. [JQL Cheatsheet] (https://cheatography.com/justinbyrne/cheat-sheets/jql-jira-query-language/)

## Raporty w JIRA
JIRA jako narzędzie do zarządzania projektem oferuje automatyczne generowanie raportów różnego typu na podstawie gotowych wzorców.
