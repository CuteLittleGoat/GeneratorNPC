# Generator NPC — dokumentacja projektu

## 1. Cel repozytorium
Projekt **Generator NPC** to osobny moduł do generowania postaci na bazie danych zewnętrznych.
Aktualna wersja UI pracuje na danych z Bestiariusza, Pancerzy i Broni oraz utrzymuje miejsce na
kolejne moduły: Psionika, Modlitwy, Talenty, Ekwipunek, Augmentacje.

## 2. Dane wejściowe
- Dane źródłowe pochodzą z pliku `data.json` w repozytorium „Repozytorium”.
- Docelowy adres źródła danych:
  - `https://cutelittlegoat.github.io/Repozytorium/data.json`

> Uwaga: środowisko pracy może wymagać dodatkowej konfiguracji CORS po stronie hostingu danych.

## 3. Wygląd i spójność UI
UI utrzymuje jednolity styl:
- nagłówki i przyciski bazują na fontach **Orbitron** i **Share Tech Mono**,
- komponenty mają półprzezroczyste tła, delikatne obramowania oraz podświetlenie akcentem,
- odnośniki do stron są formatowane klasą `.link`,
- czerwone wyróżnienia tekstu wykorzystują klasę `.text-red`,
- interpunkcja (przecinki, średniki) jest zachowywana zgodnie z danymi źródłowymi.

## 4. Funkcjonalności UI
Aktualne UI zawiera:
- wybór bazowego rekordu z Bestiariusza (realne dane z `data.json`),
- przełączniki modułów aktywnych: Pancerz, Broń,
- miejsce na moduły dodatkowe: Psionika, Modlitwy, Talenty, Ekwipunek, Augmentacje,
- tabelę z możliwością zwijania/rozwijania wierszy,
- podpowiedzi cech w panelu popover, zasilane z `_meta.traits`,
- podgląd wygenerowanej karty NPC oparty o dane bieżące.

## 5. Zmiany wprowadzane przy kolejnych aktualizacjach
Po każdej zmianie należy:
1. zaktualizować niniejszy plik opisem nowych funkcji i zmian w UI,
2. zachować spójny styl wizualny,
3. upewnić się, że mechanizm zwijania/rozwijania wierszy działa.
