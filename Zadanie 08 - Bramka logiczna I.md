# Zadanie 8 - Bramka logiczna I
![obraz](https://github.com/lech-dabrowski/mrbuggy3/assets/112244024/1cdd885e-bb4b-4460-bc22-c9138f8f8c1a)

### T1 - Testowanie wszystkich poprawnych kombinacji

**Warunki wstępne:**

Użytkownik znajduje się na stronie z bramką logiczną.

**Kroki:**

1. W pole “Wejście 1” wprowadź wartość 1
2. W pole “Wejście 2” wprowadź wartość 1
3. Kliknij na przyciszk “Oblicz”
4. Zweryfikuj poprawnośc wyniku
5. Powtórz czynności dla każdej z par: 1 i 0, 0 i 1, 0 i 0

**Oczekiwany rezultat:**

Poprawne obliczenie wyniku: 1 dla pary 1 i 1, oraz 0 dla par: 1 i 0, 0 i 1, 0 i 0

### T2 - Testowanie walidacji pól “Wejscie 1” i “Wejście 2”

**Warunki wstępne:**

Użytkownik znajduje się na stronie z bramką logiczną.

**Kroki:**

1. W pola “Wejście 1” i “Wejście 2” spróbuj wprowadzić wartości spoza poprawnej klasy równoważości:
   - liczby inne niż 0 i 1
   - litery i znaki specjalne
2. Kliknij na przyciszk “Oblicz”.

**Oczekiwany rezultat:**

Pola nie przyjmują danych wejściowych innych niż 0 i 1

[![HrYuhua.md.png](https://iili.io/HrYuhua.md.png)](https://freeimage.host/i/HrYuhua)
---
Test 2 ujawnia błąd - po kliknięciu na pole wyświetla się kursor i możliwe jest wprowadzenie dowolnego znaku z klawiatury.
