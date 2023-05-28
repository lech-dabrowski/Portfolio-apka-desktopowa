# Zadanie 4 - Formularz przelewu I

### T1 - Wszystkie dane poprawne

**Warunki wstępne:**

Użytkownik znajduje się na stronie przelewu i dysponuje Użytkownik znajduje się na stronie przelewu i dysponuje poprawnymi danymi do wykonania przelewu (w tym poprawnym numerem rachunku odbiorcy).

**Kroki:**

1. We wszystkie pola wpisz poprawne dane. Na przykład:
   - Nr. odbiorcy: 33102022251281637642546453
   - Nazwa odbiorcy: Jan Kowalski
   - Adres odbiorcy: ul. Przykładowa 123, 01-234 Miasto
   - Tytuł przelewu: Przelew środków
   - Kwota: 123.45 PLN
2. Zatwierdź dane klikając na OK
3. Zweryfikuj czy wszystkie dane są prawidłowe i kliknij na przycisk “Potwierdź” by wysłać przelew

**Oczekiwany rezultat:**

Komunikat o wykonanym przelewie i poprawna aktualizacja dostępnych środków na koncie.

### T2 - Nieudany przelew

**Warunki wstępne:**

Użytkownik znajduje się na stronie do wykonywania przelewu.

**Kroki:**

1. W jedno z pól wpisz niepoprawne dane albo pozostaw je puste
2. Zatwierdź dane klikając na OK

**Oczekiwany rezultat:**

Użytkownik zostaje poinformowany o niepoprawnych lub brakujących informacjach i nie może wysłać przelewu. Kwota na koncie nie ulega zmianie.

### T3 - Walidacja pola “Numer rachunku odbiorcy”

**Warunki wstępne:**

Użytkownik znajduje się na stronie przelewu i dysponuje poprawnymi danymi do wykonania przelewu.

**Kroki:**

1. W polu “Nr. rachunku odbiorcy” wpisz niepoprawne dane:
   - dowolną 26-cyfrową liczbę
   - liczbę krótszą bądź dłuższą
   - spróbuj wpisać litery lub znaki specjalne
   - zostaw puste pola
   - numer własnego rachunku (86 2490 0005 0000 4500 6265 9375)
2. Pozostałe pola uzupełnikj poprawnymi danymi.
3. Zatwierdź dane klikając na OK.

**Oczekiwany rezultat:**

Pole przyjmuje wyłącznie cyfry i wymaga poprawnego numeru konta. W przeciwnym razie informuje użytkownika komunikatem np. “numer rachunku jest niepoprawny”.

### T4 - Walidacja pola “Kwota”

**Warunki wstępne:**

Użytkownik znajduje się na stronie przelewu i dysponuje poprawnymi danymi do wykonania przelewu.

**Kroki:**

1. W pole “Kwota” wpisz (lub spróbuj wpisać) jedno z poniższych:
   - liczbę całkowitą bez przecinków
   - liczbę z dwoma miejscami po przecinku
   - liczbę z trzema miejscami po przecinku
   - litery i znaki specjalne
   - wartość ujemną

**Oczekiwany rezultat:**

Pole przyjmuje wyłącznie liczby z dwoma miejscami po przecinku. W przypadku wprowadzenia liczby całkowitej, automatycznie dodawane jest .00

[![HrYuhua.md.png](https://iili.io/HrYuhua.md.png)](https://freeimage.host/i/HrYuhua)
---
Test 4 ujawnia błąd. Do podanej liczby całkowitej (bez .00) dodawane jest 1.00.
