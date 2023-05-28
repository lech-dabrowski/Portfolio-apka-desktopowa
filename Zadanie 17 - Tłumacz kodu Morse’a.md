# EJ, SERIO SZKODA TWOJEGO CZASU :) ALE BARDZO DZIĘKUJĘ ZA WSPARCIE I TAK :)
# Zadanie 17 - Tłumacz kodu Morse’a

### T1 - Sprawdzanie przycisku “Sygnał”

**Warunki wstępne:**

Użytkownik znajduje się na stronie tłumacza i ma możliwość wprowadzania danych przy użyciu myszki.

**Kroki:**

1. Klikając lewym przyciskiem myszki na “Sygnał” spróbuj uzyskać następujące efekty:
   - szybkie kliknięcie odpowiadające kropce w alfabecie Morse’a
   - dłuższe kliknięcie odpowiadające kresce w alfabecie Morse’a
   - sekwencje kliknięć odpowiadające kilku znakom z tabeli
   - bardzo szybkie kliknięcia (np. cztery kropki dla H lub pięć dla 5)
   - poprawna sekwencja z przerwami dłuższymi niż 1 sekunda
   - sekwencja niewystępująca w tabeli
   - długie, kilkusekundowe wciśnięcie przycisku
2. Obserwuj zawartość okna “Kod Morse’a” by sprawdzić, czy pojawiające się znaki odpowiadają wprowadzonym danym.

**Oczekiwany rezultat:**

Program poprawnie interpretuje wprowadzone dane. Sekundowa przerwa zaczyna nowy znak a niepoprawne sekwencje są ignorowane.

### T2 - Sprawdzanie przycisku “Wyczyść”

**Warunki wstępne:**

Użytkownik znajduje się na stronie tłumacza i ma możliwość wprowadzania danych przy użyciu myszki.

**Kroki:**

1. Klikając lewym przyciskiem myszki na “Sygnał” wprowadź kilka znaków.
2. Klikając lewym przyciskiem myszki na “Wyczyść” usuń zawartość okna
3. Wprowadź kolejną sekwencję
4. Zwróć uwagę, czy okno zostało wyczyszczone oraz czy wprowadzone wcześniej znaki nie wpływają na poprawne fukcjonowanie

**Oczekiwany rezultat:**

Przycisk “Wyczyść” usuwa zawartość okna “Kod Morse’a”. Po usunięciu bieżącej zawartości, program dalej poprawnie funkcjonuje.

[![HrYuhua.md.png](https://iili.io/HrYuhua.md.png)](https://freeimage.host/i/HrYuhua)
---
Ciężko nazwać to defektem, ale jedyne zachowanie programu odbiegające od oczekiwań to czyszczenie okna “Kod Morse’a” po wciśnięciu przycisku “Sygnał” przez czas dłuższy niż 3 sekundy.
