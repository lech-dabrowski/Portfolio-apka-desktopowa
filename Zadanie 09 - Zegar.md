# Zadanie 9 - Zegar

### T1 - Walidacja pól

**Warunki wstępne:**

Użytkownik znajduje się na stronie zegara.

**Kroki:**

1. W dostępne pola wpisz dowolne wartości z przedziału 0-24 dla godzin i 0-59 dla minut.
2. Zatwierdź zmianę czasu.
3. Powtórz czynność z wartościami spoza przedziału i innymi znakami.

**Oczekiwany rezultat:**

Zegar przyjmuje tylko poprawne wartości, po zatwierdzeniu zmiany poprawnie wyświetla upływ czasu.

### T2 - Testowanie dokładności pomiaru

**Warunki wstępne:**

Użytkownik znajduje się na stronie zegara i dysponuje metodą poprawnego pomiaru czasu (stoper w telefonie, stronka Time.is, ustawienia zegara w Windowsie)

**Kroki:**

1. Zsynchronizuj czas wyświetlany w programie z tym dostępnym na drugim urządzeniu.
2. Zrób sobie kawę, herbatę lub pooglądaj memy na internecie.
3. Po upływie kilku minut sprawdź czy oba urządzenia wyświetlają ten sam czas.

**Oczekiwany rezultat:**

Oba urządzenia wyświetlają dokładnie ten sam czas

[![HrYuhua.md.png](https://iili.io/HrYuhua.md.png)](https://freeimage.host/i/HrYuhua)
---
Test 2 ujawnia błąd - testowany zegar późni się około sekundy na każda minutę.
