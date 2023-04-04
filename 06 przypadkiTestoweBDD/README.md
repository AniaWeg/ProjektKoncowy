## BDD - proces wytwarzania oprogramowania
Proces wytwarzania oprogramowania w tej technologii jest trójfazowym procesem iteracyjnym:

* na podstawie wymagań małego wycinka systemu (User story) należy przeanalizować, co dokładnie ma zostać wykonane, aby jak najpełniej zdefiniować wymagania.
* na podstawie abstrakcyjnego języka należy zautomatyzować User story.
* implementacja określonego zachowania i wykonania testów w celu weryfikacji zrealizowanych wymagań.
Idea opiera się na dokonywaniu niewielkich zmian iteracyjnie, poszerzając implementację o coraz to nowe informację. Automatyzacja ma na celu jak najefektywniejszą weryfikację sprecyzowanych wymagań.

## Zalety BDD¶
Metodologia BDD cechuje się poniższymi zaletami:

* mniejsze marnotrawstwo czasu i wysiłku - praktyki BDD wymagają skupienia wysiłków na odkrywaniu i dostarczaniu cech funkcjonalnych, które zapewniają wartość dla biznesu oraz unikaniu tych, które wartości takiej nie dostarczają.
* redukcja kosztów - dzięki skoncentrowaniu się na budowaniu cech funkcjonalnych, które mają widoczną wartość biznesową, umożliwia redukcję kosztów niezbędnych do dostarczenia produktu użytkownikowi końcowemu.
* łatwiejsze i bezpieczniejsze zmiany - dynamiczna dokumentacja generowana w ramach BDD umożliwia łatwe modyfikowanie oraz rozszerzanie aplikacji. Niskopoziomowe wymagania umożliwiają również łatwiejsze zrozumienie istniejącego kodu.
* efektywne wdrażanie zmian w kodzie - zestaw testów automatycznych powstałych, na podstawie określonych wymagań przyczyniają się również do szybszego i bezpieczniejszego wdrażania poprawek/nowych funkcjonalności w aplikacji. Testerzy nie muszą wykonywać pełnej regresji aplikacji, a mogą skupić się głównie na weryfikacji dodanych wymagań.
* jest zrozumiały dla wszystkich (PO, testerzy, interesariusze, itp), więc nie ma tutaj bariery dla osób nietechnicznych.
* wszyscy muszą myśleć w ten sam sposób/tym samym słownictwem i pojęciami.

## Wymagania BDD
Metodologia Behavior-Driven Development wymaga, by przed rozpoczęciem wdrażania zrealizowane były poniższe podpunkty

* Wymagania muszą zostać skonwertowane na User stories
* Każdy z przykładów definiujących zachowanie musi być poprawnym i konkretnym przykładem.
* Znajomość języka dokumentacji zachowań.
* Przestawienie myślenia z programowania sterowanego testami, na programowanie sterowane zachowaniami.

## Problemy związane z BDD
* stosowanie praktyk BDD wymaga dużego zaangażowania każdej ze stron zespołu, co niejednokrotnie wymaga czasu niezbędnego na dyskusję. Brak dyskusji i zaangażowania nie pozwoli na zwinną realizację produktu.
* praktyki BDD realizuje się najlepiej na podstawie metodologii zwinnych
* praktyki nie sprawdzają się dobrze w projektach typu silos (z ang. siloed development), gdzie różne zespoły odpowiedzialne są za różne fazy produktu. Separacja i brak komunikacji pomiędzy nimi praktycznie uniemożliwia wydajne i efektywne precyzowanie wymagań
* źle napisane testy mogą znacznie zwiększyć koszty utrzymania produktu ze względu na potrzebę utrzymania testów, które ulegają dewaluacji przy każdej zmianie skorelowanych wymagań

