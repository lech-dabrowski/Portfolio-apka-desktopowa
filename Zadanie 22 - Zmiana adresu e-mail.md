# Zadanie 22 - Zmiana adresu e-mail

### T1 - Poprawne działanie

**Warunki wstępne:**

Użytkownik znajduje się na stronie formularza umożliwiającego zmianę adresu.

**Kroki:**

1. W pole “Aktualny adres e-mail” wprowadź zawartośc pola “Aktywny adres e-mail”
2. W pole “Nowy adres e-mail” wprowadź dane w poprawnym formacie (przykład@domena.xx)
3. Klikając na przycisz “Zmień” zatwierdź zmianę adresu
4. Obserwuj czy zawartość pola “Aktywny adres e-mail” została poprawnie zmieniona

**Oczekiwany rezultat:**

Formularz umożliwia zmianę aktywnego adresu poprzez sprawdzenie aktualnego i podanie nowego adresu e-mail.

### T2 - Walidacja pola “Aktualny adres e-mail”

**Warunki wstępne:**

Użytkownik znajduje się na stronie formularza umożliwiającego zmianę adresu.

**Kroki:**

1. W pole “Aktualny adres e-mail” wprowadź niepoprawne dane:
   - inny adres w poprawnym formacie
   - dowolny ciąg znaków
   - dane w poprawnym formacie, ale ze znakami specjalnymi
2. W pole “Nowy adres e-mail” wprowadź dane w poprawnym formacie (przykład@domena.xx)
3. Klikając na przycisz “Zmień” zatwierdź zmianę adresu
4. Obserwuj czy zawartość pola “Aktywny adres e-mail” została poprawnie zmieniona

**Oczekiwany rezultat:**

Formularz nie pozwala na zmianę adresu, jeżeli w pierwszym polu nie jest podany obecny adres.

### T3 - Walidacja pola “Nowy adres e-mail”

**Warunki wstępne:**

Użytkownik znajduje się na stronie formularza umożliwiającego zmianę adresu.

**Kroki:**

1. W pole “Aktualny adres e-mail” wprowadź zawartośc pola 
2. W pole “Nowy adres e-mail” wprowadź niepoprawne dane:
   - inny adres w poprawnym formacie
   - dowolny ciąg znaków
   - dane w poprawnym formacie, ale ze znakami specjalnymi
   - adres identyczny z tym w polu “Aktywny adres e-mail”
3. Klikając na przycisz “Zmień” zatwierdź zmianę adresu
4. Obserwuj czy zawartość pola “Aktywny adres e-mail” została poprawnie zmieniona

**Oczekiwany rezultat:**

Formularz nie pozwala na zmianę adresu, jeżeli w nowy adres jest niepoprawny

### T4 - Nadpisywanie danych

**Warunki wstępne:**

Użytkownik znajduje się na stronie formularza umożliwiającego zmianę adresu.

**Kroki:**

1. Przeprowadź poprawną zamianę adresu wg. T1 zapamiętując pierwotny adres
2. Wykonaj ponownie te same kroki, by przywrócić zastąpić nowy adres pierwotnym
3. Klikając na przycisz “Zmień” zatwierdź zmianę adresu
4. Obserwuj czy zawartość pola “Aktywny adres e-mail” została poprawnie zmieniona

**Oczekiwany rezultat:**

Wg wymagań formularz przechowuje w pamięci tylko jeden adres, więc można bez problemu przywrócić adres użyty wcześniej.

[![HrYuhua.md.png](https://iili.io/HrYuhua.md.png)](https://freeimage.host/i/HrYuhua)
---
T4 wykazuje błąd: raz użyty adres pozostaje w bazie i nie jest możliwe jego ponowne użycie, co jest niezgodne z wymaganiami.
