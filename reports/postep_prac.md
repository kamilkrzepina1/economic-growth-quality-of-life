
# Postęp projektu – 8 listopada 2026

## Temat
Wzrost gospodarczy a jakość życia w krajach Unii Europejskiej – analiza statystyczna danych społeczno-ekonomicznych w latach 2010–2024.

## Zrealizowane zadania

- Przygotowano środowisko Python i Jupyter Notebook.
- Skonfigurowano biblioteki do analizy danych.
- Pobrano dane o wzroście realnego PKB na mieszkańca dla UE-27.
- Pobrano dane o medianie dochodu w PPS dla UE-27.
- Sprawdzono ograniczenia PPS w analizie zmian dochodu w czasie.
- Pobrano medianę dochodu w walutach krajowych (NAC).
- Pobrano indeks HICP dla Polski i Niemiec.
- Przygotowano funkcję `get_hicp_data()`.
- Pobrano dane HICP dla UE-27.
- Przygotowano testowe obliczenie realnej mediany dochodu dla Polski w cenach z 2015 r.

## Zapisane zbiory danych

- `data/processed/gdp_growth_eu27_2010_2024.csv`
- `data/processed/eu_gdp_income_2010_2024.csv`
- `data/processed/poland_real_income_2010_2024.csv`
- `data/processed/eu_hicp_2010_2024.csv`

## Następne zadania

1. Pobrać medianę dochodu w walutach krajowych dla wszystkich 27 państw.
2. Dopasować lata dochodu do właściwych lat odniesienia.
3. Obliczyć realną medianę dochodu dla UE-27.
4. Sprawdzić kompletność i poprawność danych.
5. Połączyć dane o dochodach z danymi o PKB.
6. Przejść do analizy statystycznej.
7. ### Zależność między wzrostem gospodarczym a zmianą wskaźnika zatrudnienia

Analiza 27 państw Unii Europejskiej wykazała silną dodatnią korelację między średnim tempem wzrostu realnego PKB per capita w latach 2010–2024 a zmianą wskaźnika zatrudnienia osób w wieku 20–64 lat w tym samym okresie.

### Wyniki regresji – wzrost PKB a zmiana wskaźnika AROPE

Wyniki regresji liniowej wskazują na ujemną i statystycznie istotną zależność pomiędzy średniorocznym wzrostem realnego PKB na mieszkańca a zmianą wskaźnika AROPE w krajach UE w latach 2015–2024. Współczynnik regresji wyniósł -1,9158 (p < 0,001). Oznacza to, że wzrost średniorocznego tempa wzrostu PKB na mieszkańca o 1 punkt procentowy wiązał się przeciętnie ze spadkiem wskaźnika AROPE o około 1,92 punktu procentowego. Współczynnik determinacji R² wyniósł 0,408, co oznacza, że model opisuje 40,8% zróżnicowania zmian wskaźnika AROPE pomiędzy analizowanymi państwami. Wyniki wskazują, że wyższemu wzrostowi gospodarczemu towarzyszyła przeciętnie większa poprawa w zakresie zagrożenia ubóstwem lub wykluczeniem społecznym. Nie pozwalają jednak na stwierdzenie związku przyczynowo-skutkowego.

### Wyniki regresji – wzrost PKB a zmiana oczekiwanej długości życia

Wyniki regresji liniowej wskazują na dodatnią i statystycznie istotną zależność pomiędzy średniorocznym wzrostem realnego PKB na mieszkańca a zmianą oczekiwanej długości życia w krajach UE w latach 2010–2024. Współczynnik regresji wyniósł 0,2806 (p = 0,00972). Oznacza to, że wzrost średniorocznego tempa wzrostu PKB na mieszkańca o 1 punkt procentowy wiązał się przeciętnie ze wzrostem oczekiwanej długości życia o około 0,28 roku. Współczynnik determinacji R² wyniósł 0,239, co oznacza, że model opisuje 23,9% zróżnicowania zmian oczekiwanej długości życia pomiędzy analizowanymi państwami. W porównaniu z pozostałymi analizowanymi wymiarami jakości życia zależność ta była słabsza. Wynik nie pozwala na stwierdzenie związku przyczynowo-skutkowego.

Współczynnik korelacji Pearsona wyniósł **r = 0,810** (p < 0,001), natomiast współczynnik korelacji rang Spearmana osiągnął **ρ = 0,818** (p < 0,001). Oba wyniki wskazują na silną dodatnią zależność: państwa o wyższym średnim tempie wzrostu gospodarczego miały na ogół również większy wzrost wskaźnika zatrudnienia.

Zbliżone wartości obu współczynników sugerują, że zaobserwowana zależność nie ogranicza się wyłącznie do liniowego układu danych i jest widoczna również przy porównywaniu rang państw.

Należy jednak podkreślić, że analiza ma charakter korelacyjny. Nie pozwala stwierdzić, że wzrost PKB bezpośrednio powoduje wzrost zatrudnienia. Na oba zjawiska mogą wpływać również inne czynniki gospodarcze, społeczne i demograficzne.