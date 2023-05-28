# Zadanie 10 - Lista produktów I

### T1 - Poprawne dodanie produktu

**Warunki wstępne:**

Użytkownik znajduje się na stronie listy i ma możliwość dodawania produktów.

**Kroki:**

1. Uzupełnij pola “Nazwa”, “Ilość”, “Cena netto” oraz “Stawka VAT” poprawnymi wartościami.
2. Kliknij “Dodaj produkt” by utworzyć nową pozycję na liście
3. Obserwuj czy wszystkie wartości są poprawnie przenoszone do odpowiednich komórek tabeli.

**Oczekiwany rezultat:**

Program poprawnie dodaje produkty do listy. Wartości podane przez użytkownika trafiają w odpowiednie kolumny.

### T2 - Sortowanie listy

**Warunki wstępne:**

Użytkownik znajduje się na stronie listy i ma utworzonych przynajmniej 5 produktów.

**Kroki:**

1. Klikając na nagłówek kolumny “Nazwa” posortuj listę alfabetycznie
2. Zwróć uwagę czy wartości w pozostałych kolumnach poprawnie się zmieniają.

**Oczekiwany rezultat:**

Program poprawnie sortuje listę produktów wg wszystkich kolumn. Wartości raz przypisane do produktu nie ulegają zmianie.

### T3 - Walidacja pól

**Warunki wstępne:**

Użytkownik znajduje się na stronie listy i ma możliwość dodawania produktów.

**Kroki:**

1. W pola “Ilość”, “Cena netto” spróbuj wpisać dane inne niż liczby całkowite lub ułamkowe z dwoma miejscami po przecinku.
2. Pozostałe pola uzupełnij poprawnymi danymi.
3. Kliknij “Dodaj produkt” by utworzyć nową pozycję na liście

**Oczekiwany rezultat:**

Jedyne wartości, jakie możemy wpisać w pola numeryczne to cyfry od 0 do 9 i przecinek. 

### T4 - Sprawdzanie poprawności obliczeń

**Warunki wstępne:**

Użytkownik znajduje się na stronie z listą produktów i ma możliwość wykonywania poprawnych obliczeń np. przy użyciu kalkulatora.

**Kroki:**

1. Dodaj do listy produkty, których cena i ilość pozwolą na przetestowanie następujących obliczeń:
   1. Zaokrąglanie liczb do drugiego miejsca po przecinku
   2. Obliczenia na dużych liczbach
   3. Konwersja liczby całkowitej na zmiennoprzecinkową
2. Zwróć uwagę czy wartości generowane w polach “Wartość netto”, “Wartość VAT” oraz “Wartość brutto” są kalkulowane prawidłowo.

**Oczekiwany rezultat:**

Program poprawnie kalkuluje wszystkie wartości. Wyniki są zaokrąglane do drugiego miejsca po przecinku.

[![HrYuhua.md.png](https://iili.io/HrYuhua.md.png)](https://freeimage.host/i/HrYuhua)
---
Test 2 ujawnia błąd - kolejność liczb w pierwszej kolumnie ”L.p.” nie zmienia się zależnie od sortowania, co skutkuje niepoprawnym przypisywaniem liczby porządkowej.

[![HrYuhua.md.png](https://iili.io/HrYuhua.md.png)](https://freeimage.host/i/HrYuhua)
---
Test 4 ujawnia błąd - przy stawce VAT 8% wyniki nie są zaokrąglane.
