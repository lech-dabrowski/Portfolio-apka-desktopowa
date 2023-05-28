# Zadanie 18 - Bramka logiczna II

[![HrYuhua.md.png](https://iili.io/HrYuhua.md.png)](https://freeimage.host/i/HrYuhua)
---
Powtórzono testy z [Zadania 8](https://github.com/lechdabrowski42/mrbuggy3/blob/main/Zadanie%2008%20-%20Bramka%20logiczna%20I.md). Test 2 ujawnia błąd - po kliknięciu na pole nadal wyświetla się kursor i możliwe jest wprowadzenie dowolnego znaku z klawiatury.

[![HrYuhua.md.png](https://iili.io/HrYuhua.md.png)](https://freeimage.host/i/HrYuhua)
---
Część błędnych kombinacji jest co prawda walidowana i wyświetlany jest stosowny komunikat, ale nadal możliwe jest wprowadzenie dwóch jednakowych znaków (niebędących 0 lub 1) co zwróci błędny wynik 2.
