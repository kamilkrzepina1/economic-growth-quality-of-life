
# Wzrost gospodarczy a jakość życia w krajach Unii Europejskiej

## Temat badania

**Wzrost gospodarczy a jakość życia w krajach Unii Europejskiej –
analiza statystyczna danych społeczno-ekonomicznych w latach 2010–2024.**

## Cel badania

Celem projektu jest zbadanie zależności statystycznych między
wzrostem gospodarczym a wybranymi wymiarami jakości życia
w 27 państwach Unii Europejskiej w latach 2010–2024.

Analiza ma charakter ilościowy, porównawczy i obserwacyjny.
Jednostką obserwacji jest kraj w danym roku.

## Zakres badania

- 27 państw Unii Europejskiej.
- Okres analizy: 2010–2024.
- Dane roczne.
- Źródło danych: Eurostat.
- Analiza przekrojowa i panelowa.

## Wykorzystane wskaźniki

1. Roczna stopa wzrostu realnego PKB per capita.
2. Mediana ekwiwalentnego dochodu do dyspozycji.
3. Wskaźnik zatrudnienia osób w wieku 20–64 lata.
4. Wskaźnik zagrożenia ubóstwem lub wykluczeniem społecznym (AROPE).
5. Oczekiwana długość życia w chwili urodzenia.

Dodatkowo skonstruowano syntetyczny indeks jakości życia
oparty na dochodach, zatrudnieniu, wskaźniku AROPE
i oczekiwanej długości życia.

## Metody badawcze

- Statystyki opisowe.
- Korelacja Pearsona.
- Korelacja rang Spearmana.
- Prosta regresja liniowa OLS.
- Modele panelowe z efektami stałymi krajów i lat.
- Błędy standardowe klastrowane według krajów.
- Analiza wrażliwości leave-one-country-out.
- Standaryzacja wskaźników i konstrukcja indeksu syntetycznego.

## Najważniejsze wyniki

W analizie przekrojowej stwierdzono dodatnie zależności
między wzrostem PKB a wzrostem realnych dochodów
(r = 0,866) oraz zmianą wskaźnika zatrudnienia (r = 0,810).

Zaobserwowano również ujemną zależność między wzrostem PKB
a zmianą wskaźnika AROPE (r = -0,638).

Zależność między wzrostem PKB a zmianą oczekiwanej długości
życia była umiarkowanie dodatnia (r = 0,489).

W przypadku syntetycznego indeksu jakości życia uzyskano
ujemną korelację przekrojową (r = -0,611), natomiast
w modelu panelowym stwierdzono dodatnią zależność
z opóźnionym wzrostem PKB.

Wyniki wskazują, że zależności między wzrostem gospodarczym
a jakością życia różnią się w zależności od analizowanego
wymiaru.

## Ograniczenia

Badanie ma charakter obserwacyjny, dlatego nie pozwala
na wnioskowanie przyczynowo-skutkowe.

Indeks jakości życia obejmuje lata 2015–2024 i 26 państw.
Jest standaryzowany osobno dla każdego roku, a zatem
odzwierciedla względną pozycję państw w badanej grupie.

## Struktura projektu

- `data/raw/` – surowe dane źródłowe.
- `data/processed/` – przetworzone zbiory danych i zestawienia wyników.
- `figures/` – wykresy i wizualizacje.
- `notebooks/` – notebooki Jupyter.
- `reports/` – raporty i dokumentacja badania.

## Uruchomienie projektu

Projekt przygotowano w Pythonie i Jupyter Notebook.

Wymagane biblioteki znajdują się w pliku `requirements.txt`.

## Autorstwo i źródło danych

Dane statystyczne pochodzą z bazy Eurostat.
