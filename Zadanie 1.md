# Mr. Buggy

<aside>
💡 Najważniejszym celem poniższych przypadków testowych jest zilustrowanie procesu myślowego, jaki towarzyszył mi w poszukiwaniu błędów w trzeciej edycji aplikacji MrBuggy. Stąd w wielu miejscach podane są przykłady, a czynność raz opisana ze szczegółami, w kolejnych testach nie jest dokładnie opisywana.

</aside>

# Zadanie 1 - Rejestracja użytkownika

### T1 - Wszystkie dane poprawne

**Warunki wstępne:**

Użytkownik znajduje się na stronie rejestracji i dysponuje danymi potrzebnymi do poprawnej rejestracji.

**Kroki:**

1. We wszystkie pola wpisz poprawne dane. Na przykład:
   - jkowalski
   - silne hasło: h$SCg@VuXy9dU59zz
   - poprawnie powtórzone hasło
   - Jan
   - Kowalski
2. Spróbuj zarejestrować użytkownika klikając na przycisk.

**Oczekiwany rezultat:**

Rejestracja przebiega pomyślnie i wyświetla się komunikat potwierdzający rejestrację.

### T2 - Nazwa użytkownika - poprawne

**Warunki wstępne:**

Użytkownik znajduje się na stronie rejestracji i dysponuje danymi potrzebnymi do poprawnej rejestracji.

**Kroki:**

1. W pole “Nazwa użytkownika” wpisz wszystkie typy wartości, które powinny być poprawne wg założeń. Np.:
   - jkowalski, j_kowalski, j-kowalski, 62nu7VhghoOq8Ij24
2. Pozostałe pola uzupełnij poprawnymi danymi.
3. Spróbuj zarejestrować użytkownika klikając na przycisk.

**Oczekiwany rezultat:**

Rejestracja przebiega pomyślnie i wyświetla się komunikat potwierdzający rejestrację.

### T3 - Nazwa użytkownika - niepoprawne

**Warunki wstępne:**

Użytkownik znajduje się na stronie rejestracji i dysponuje danymi potrzebnymi do poprawnej rejestracji.

**Kroki:**

1. W pole “Nazwa użytkownika” wpisz wszystkie typy wartości, które wg założeń nie będą poprawne. Na przykład:
   - jan, jan kowalski, j.kowalski, jankówąlśki
2. Pozostałe pola uzupełnij poprawnymi danymi.
3. Spróbuj zarejestrować użytkownika klikając na przycisk.

**Oczekiwany rezultat:**

Rejestracja się nie powodzi. Wyświetlany zostaje komunikat pomagający zidentyfikować kłopot (np. “nazwa użytkownika nie powinna zawierać znaków specjalnych”).

### T4 - Hasło - niepoprawne

**Warunki wstępne:**

Użytkownik znajduje się na stronie rejestracji i dysponuje danymi potrzebnymi do poprawnej rejestracji.

**Kroki:**

1. W pole “Hasło” wpisz warości niezgodne z polityką haseł.
   - Hasło zbyt krótkie, ale ze wszystkimi wymaganymi znakami.
   - Hasło długie, ale bez wymaganych znaków
2. Pozostałe pola uzupełnij poprawnymi danymi.
3. Spróbuj zarejestrować użytkownika klikając na przycisk.

**Oczekiwany rezultat:**

Rejestracja się nie powodzi. Wyświetlany zostaje komunikat pomagający zidentyfikować problem (np. “hasło jest za słabe”).

### T5 - Hasło - błąd przy powtórzeniu hasła

**Warunki wstępne:**

Użytkownik znajduje się na stronie rejestracji i dysponuje danymi potrzebnymi do poprawnej rejestracji.

**Kroki:**

1. W pole “Hasło” wpisz poprawne hasło.
2. W pole “Powtórz hasło” wpisz hasło błędnie
3. Pozostałe pola uzupełnij poprawnymi danymi.
4. Spróbuj zarejestrować użytkownika klikając na przycisk.

**Oczekiwany rezultat:**

Rejestracja się nie powodzi. Wyświetlany zostaje komunikat pomagający zidentyfikować problem (np. “podane hasła różnią się od siebie”).

### T6 - Walidacja pól - długi ciąg znaków

**Warunki wstępne:**

Użytkownik znajduje się na stronie rejestracji i dysponuje danymi potrzebnymi do poprawnej rejestracji.

**Kroki:**

1. Poprawne dane jednego z pól zastąp bardzo długim ciągiem znaków, na przykład: 
   - 62nu7VhghoOq8Ij24fKDl9K3RO6I8s8rNx9KgsiV3uZwbe0nr3psqYSqHYKZGYcuW7LCMaxrEM5vqeHjDYJHsDZ5kRZbYTrmyQTg62nu7VhghoOq8Ij24fKDl9K3RO6I8s8rNx9KgsiV3uZwbe0nr3psqYSqHYKZGYcuW7LCMaxrEM5vqeHjDYJHsDZ5kRZbYTrmyQTg62nu7VhghoOq8Ij24fKDl9K3RO6I8s8rNx9KgsiV3uZwbe0nr3psqYSqHYKZGYcuW7LCMaxrEM5v
2. Pozostałe pola uzupełnij poprawnymi danymi.
3. Spróbuj zarejestrować użytkownika klikając na przycisk.

**Oczekiwany rezultat:**

Rejestracja się nie powodzi. Wyświetlany zostaje komunikat informujący o limicie znaków.

### T7 - Walidacja pól - puste pola

**Warunki wstępne:**

Użytkownik znajduje się na stronie rejestracji i dysponuje danymi potrzebnymi do poprawnej rejestracji.

**Kroki:**

1. Pole “Nazwa użytkownika” pozostaw puste.
2. Pozostałe pola uzupełnij poprawnymi danymi.
3. Spróbuj zarejestrować użytkownika klikając na przycisk.
4. Powtórz czynność dla każdego z pól.

**Oczekiwany rezultat:**

Rejestracja się nie powodzi. Wyświetlany zostaje komunikat identyfikujący puste pole.

### T8 - Walidacja pól - Imię i nazwisko

**Warunki wstępne:**

Użytkownik znajduje się na stronie rejestracji i dysponuje danymi potrzebnymi do poprawnej rejestracji.

**Kroki:**

1. W pola “Imię” oraz “Nazwisko” wpisz niecodzienne znaki (wg wymagań oba pola mają przyjmować wszystkie znaki)
2. Pozostałe pola uzupełnij poprawnymi danymi.
3. Spróbuj zarejestrować użytkownika klikając na przycisk.

**Oczekiwany rezultat:**

Rejestracja zakończona powodzeniem.

<aside>
🪲 Test 7 ujawnia błąd. Formularz przyjmuje dowolną ilość pustych pól.

</aside>

<aside>
💡 O ile wynik Testu 6 nie jest błędem, zaleca się wprowadzenie rozsądnego limitu znaków by uniknąć nadmiernego wzrostu rozmiaru bazy danych.

</aside>
