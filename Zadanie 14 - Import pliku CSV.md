# Zadanie 14 - Import pliku CSV

### T1 - Poprawny import pliku

**Warunki wstępne:**

Użytkownik znajduje się na stronie narzędzia do importowania plików CSV. Dysponuje możliwością tworzenia i edytowania plików CSV np. przy pomocy programu Excel.

**Kroki:**

1. Utwórz plik, z wartościami dla następujących kolumn: id, Nazwa, Osoba, Telefon, Fax, Ulica, Miejscowość, Kod, Kraj. Wartości nie muszą odpowiadać
2. Wyeksportuj plik zaznaczając opcję użycia przecinka w roli separatora.
3. Zaimportuj przygotowany plik klikając na przycisk “Wczytaj CSV” i nawigując do odpowiedniego pliku na dysku.
4. Obserwuj czy wszystkie kolumny tabelki są uzupełniane odpowiednimi wartościami z pliku.

**Oczekiwany rezultat:**

Program poprawnie importuje wszystkie wartości.

### T2 - Import dużego pliku

**Warunki wstępne:**

Użytkownik znajduje się na stronie narzędzia do importowania plików CSV. Dysponuje tabelką z kilkudziesięcioma wpisami (dopuszczalne jest kopiowanie danych - ważne, aby każdy wpis miał sekwencyjny numer ID oraz unikalne, zgodne z wymaganiami dane w każdej kolumnie)

**Kroki:**

1. Zaimportuj nowy plik klikając na przycisk “Wczytaj CSV” i nawigując do odpowiedniego pliku na dysku.
2. Obserwuj czy wszystkie kolumny tabelki są uzupełniane odpowiednimi wartościami zwracając szczegolną uwagę na:
   - poprawne sortowanie wartości
   - poprawny import wartości w kolumnach
   - poprawne wyświetlanie wszystkich znaków

**Oczekiwany rezultat:**

Program poprawnie importuje wszystkie wartości. Możliwe jest sortowanie po każdej z kolumn, pozostałe wartości w obrębie wiersza zmianiają się odpowiednio. Wszystkie dane wyświeltają się prawidłowo.

### T3 - Walidacja pól

********************Wymagania:********************

W wytycznych do zadania nie podano jakie wartości powinna przyjmować każda z kolumn, ale mając na uwadze dobre praktyki stosowane w takich sytuacjach, przyjmujemy co następuje:

Kolumna ID przyjmuje tylko liczby całkowite.

Kolumny Nazwa, Osoba kontaktowa, Miejscowość i Kraj przyjmują litery i znaki specjalne (na wypadek apostrofów i myślników w nazwiskach)

Kolumny Telefon, Fax i Kod pocztowy przyjmują cyfry i znaki specjalne

Kolumna Ulica przyjmuje Litery, cyfry i znaki specjalne (na wypadek apostrofów i myślników w nazwach ulic)

**Warunki wstępne:**

Użytkownik znajduje się na stronie narzędzia do importowania plików CSV. Dysponuje możliwością tworzenia i edytowania plików CSV np. przy pomocy programu Excel.

**Kroki:**

1. Zmodyfikuj kilka wierszy w używanym pliku, by uwzględnić niepoprawne wartości:
   - Litery i znaki specjalne w polu ID
   - Cyfry i znaki specjalne w polach nazw
   - Litery w polach liczbowych
   - Bardzo długie wpisy (mozna wykorzystać ciąg znaków z T6 zadania 1)
2. Zaimportuj zmodyfikowany plik klikając na przycisk “Wczytaj CSV” i nawigując do odpowiedniego pliku na dysku.
3. Obserwuj czy wyświetlany jest komunikat błędu o niepoprawnych danych, czy zainportowane wartości są poprawnie wyświetlane.

**Oczekiwany rezultat:**

Najbardziej rygorystyczne wymagania stawiamy polu ID - cokolwiek innego niż cyfry w tym polu to błąd krytyczny. Niepoprawne wartości w pozostałych polach będziemy traktować jako błędy o niskim priorytecie.

[![HrYuhua.md.png](https://iili.io/HrYuhua.md.png)](https://freeimage.host/i/HrYuhua)
---
T2 wskazuje błąd w wyświetlaniu numerów FAX - w co dziewiątej kolumnie zamiast faxu wyświetlany jest numer telefonu.

[![HrYuhua.md.png](https://iili.io/HrYuhua.md.png)](https://freeimage.host/i/HrYuhua)
---
T3 ujawnia, że żadne z pól nie jest walidowane - można umieszczać w nich dowolne znaki w dowolnej ilości. Jest to poważny błąd w przypadku pola ID.

💡 Testowanie dodatkowo ujawniło, że pliki zakodowane w ANSI nie wyświetlają poprawnie dnaków diaktrycznych. Problem nie występuje w UTF-8

