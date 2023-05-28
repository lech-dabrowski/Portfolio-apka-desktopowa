# Zadanie 15 - Galeria obrazków I

### T1 - Poprawna generacja galerii

**Warunki wstępne:**

Użytkownik znajduje się na stronie narzędzia do generowania galerii ze zdjęć i dysponuje sześcioma obrazkami spełniającymi wymagania w obu formatach (np. trzy .jpg i trzy .png).

**Kroki:**

1. Kliknij na przycisk “Wczytaj” by otworzyć okno importu i nawiguj do katalogu z obrazkami. 
2. Zaimportuj poprawnie przygotowany obrazek klikając na “Otwórz”.
3. Powtórz czynność dla pozostałych pięciu pól.
4. Kliknij na “Generuj” by utworzyć kompozycję z obrazków.
5. Obserwuj czy obrazki wczytane zostały prawidłowo i we wskazanej kolejności.

**Oczekiwany rezultat:**

Program poprawnie importuje obrazki w wymaganych formatach i generuje kompozycję na siatce 3 x 2

### T2 - Wczytywanie mniejszych obrazków

**Warunki wstępne:**

Użytkownik znajduje się na stronie narzędzia do generowania galerii ze zdjęć i dysponuje sześcioma plikami graficznymi w poprawnym formacie i o różnych wymiarach nie przekraczających 200x200 pikseli. 

**Kroki:**

1. Klikając na “Wczytaj” zaimportuj po obrazku w każde z sześciu pól.
2. Kliknij na “Generuj” by utworzyć kompozycję z obrazków.
3. Obserwuj czy obrazki wczytane zostały prawidłowo

**Oczekiwany rezultat:**

Program  radzi sobie z róznymi rozmiarami i poprawnie generuje kompozycję na siatce 3 x 2

### T3 - Wczytywanie obrazków niezgodnych z wymaganiami

**Warunki wstępne:**

Użytkownik znajduje się na stronie narzędzia do generowania galerii ze zdjęć i posiada możliwość edytowania rozszerzeń i rozmiarów plików graficznych w innym programie.

**Kroki:**

1. Kliknij na przycisk “Wczytaj” by otworzyć okno importu wskaż do zaimportowania niepoprawne pliki:
   - Obrazki, których jeden lub dwa boki przekraczają 200 pikseli.
   - Pliki graficzne o innych rozszerzeniach (.bmp, .tiff, .gif).
   - Pliki niebędące grafikami (.txt, .xls, .exe).
2. Spróbuj zaimportować obrazek klikając na “Otwórz”.
3. Sprawdź czy import jest możliwy oraz obserwuj wyświetlane komunikaty.

**Oczekiwany rezultat:**

Program poprawnie identyfikuje niepoprawne pliki i wyświetla stosowny komunikat (np. “wymiar pliku powyżej 200 pikseli” albo “niepoprawny format pliku”)

### T4 - Walidacja nazw i rozszerzeń plików

**Warunki wstępne:**

Użytkownik znajduje się na stronie narzędzia do generowania galerii ze zdjęć i dysponuje sześcioma obrazkami spełniającymi wymagania.

**Kroki:**

1. Zmień nazwy poprawnie przygotowanych plików, by uwzględnić następujące scenariusze:
   - nazwy ze znakami diaktrycznymi
   - nazwy zawierające znaki białe i specjalne
   - nazwa i rozszerzenie napisane wielkimi literami
   - bardzo długa nazwa
   - manualnie usunięte rozszerzenie pliku
2. Nawiguj do utworzonych plików i importuj obrazki klikając na “Otwórz”
3. Obserwuj czy pliki są importowane i ewentualne komunikaty o błędach.
4. Wygeneruj galerię ze zdjęć klikając na “Generuj”

**Oczekiwany rezultat:**

Program poprawnie importuje pliki z różnymi znakami w nazwie i ewentualne problemy są indentfikowane, a użytkownik jest informowany stosownym komunikatem.

[![HrYuhua.md.png](https://iili.io/HrYuhua.md.png)](https://freeimage.host/i/HrYuhua)
---
Błąd występuje w T4 - pliki o rozszerzeniu JPG lub PNG (wielkie litery) są poprawnie importowane (nie wyświetla się komunikat o błędzie), ale nie pojawiają się w wygenerowanej galerii.
