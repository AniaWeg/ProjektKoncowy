Jak ze zwykłej i nieuporządkowanej specyfikacji 🤯 uzyskać wysokojakościowe kryteria akceptacji 🤗 ...?

Tutaj przyjdzie nam z pomocą metodologia wytwarzania oprogramowania 👉 **BDD (Behavior Driven Develpment)**

Podstawą tej metody jest próba jak najpełniejszego poznania potrzeb, celów i wymagań klienta oraz przygotowania oprogramowania spełniającego te kryteria.
Testy skupiają się nie tyle na konkretnej implementacji, a raczej na konkretnych zachowaniach , które muszą zostać zrealizowane w ramach implementowanego rozwiązania. Zachowania opisywane są w abstrakcyjnym języku z perspektywy klienta, a jego składnia przypomina język naturalny, co ułatwia jego specyfikację i analizę przez osoby nietechniczne. Zachowania opierają się zazwyczaj o historyjki użytkownika (**user stories**)

*"Jako **[rola]**..., chcę **[funkcja]**..., by **[korzyść]**..."*

*"As a **[role]**..., I want **[action]**..., so that **[benefit]**..."*

**rola** - typ użytkowanika, który powinien dokonywać interakcji w systemie. Należy określić typ użytkownika możliwie precyzyjnie mając na uwadze, że espól deweloperski nie jest użytkownikiem.

**funkcja** - rodzaj zachowania do implementacji w systemie. Akcja ta powinna być unikalna dla danej _User Story_

**korzyść** - określona korzyść powinna być rezultatem wykonania historyjki. Wiele _User Stories_ może dzieli te same korzyści.


👇
Kryterium akceptacji może przybrać np.: taką formę:

*"Zakładając, że..., jeśli..., to (wtedy)..."*

*"Given..., when..., then..."*
