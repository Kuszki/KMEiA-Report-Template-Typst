# Szablon sprawozdania z ćwiczenia w laboratorium KMEiA

Niniejszy szablon przeznaczony jest do formatowania sprawozdania zgodnie z wytycznymi obowiązującymi w Katedrze Metrologii, Elektroniki i Automatyki Wydziału Elektrycznego Politechniki Śląskiej.

Projekt wykorzystuje tylko i wyłącznie wolne oprogramowanie i zachęca użytkowników do stosowania go podczas codziennej pracy. Celem projektu jest również zachęcenie odbiorców do stosowania systemu składu `Typst` podczas tworzenia dokumentów, jako alternatywy dla klasycznych edytorów tekstu, które mimo pozornie łatwiejszej obsługi, nie oferują tak dużej prostoty, swobody i jakości sporządzania dokumentów. O ile próg wejścia w `LaTeX` jest dość wysoki, o tyle dotyczy to głównie tworzenia tego typu szablonu, a nie stosowania ich.

**UWAGA** - nie jest to oficjalny szablon sprawozdania - oficjalny szablon dostępny jest na [stronie Katedry](https://www.polsl.pl/re2/materialy).

## Struktura katalogów

Szablon złożony jest z następujących katalogów:
* `obrazki` – tutaj zaleca się umieszczanie obrazków i rysunków,
* `wyniki` – tutaj znajdują się pliki z wynikami pomiarów i obliczeń.

## Pliki w katalogu głównym

W katalogu głównym znajdują się następujące pliki:
* `report.typ` – klasa szablonu dokumentu (nie należy edytować),
* `main.typ` – główny plik dokumentu (należy uzupełnić).

## Podstawowe opcje szablonu

W pliku `main.typ` należy uzupełnić dane dotyczące pracy, zgodnie z komentarzami w pliku, a następnie dodać kolejne rozdziały pracy. Poza opcjami wskazanymi bezpośrednio w omawianym pliku, istnieje również możliwość ustawienia opcji:
* `bibfile` – ścieżka pliku z bibliografią, domyślnie `none`,
* `bibstyle` – styl bibliografii, domyślnie `ieee`,
* `headstyle` – wersja nagłówka dokumentu, domyślnie `default`, możliwe opcje: `default`, `compact`,
* `margin` – rozmiar marginesów, domyślnie `1.75cm`,
* `font-sans` – czcionka bezszeryfowa, domyślnie `Latin Modern Sans`,
* `font-mono` – czcionka o stałej szerokości, domyślnie `Latin Modern Mono`,
* `font-math` – czcionka stosowana w równaniach, domyślnie `Latin Modern Math`,
* `font-size` – główny rozmiar czcionki, domyślnie `12pt`,

Pliku `report.typ` nie zaleca się edytować – można to jednak zrobić, jeśli konieczna jest edycja stylu dokumentu i dostosowanie go do własnych preferencji. W tym celu najeży jednak posiadać pewną wiedzę i wprawę w stosowaniu `Typst`.

## Kompilacja dokumentu

Niniejszy szablon może być stosowany bezpośrednio w serwisie [`typst.app`](https://typst.app). Zaleca się jednak, z uwagi na ochronę własności intelektualnej i zapobieganie analizowaniu dokumentu przez obce podmioty, instalację kompilatora `Typst` na własnym komputerze. Kompilator ten dostępny jest w zasadzie dla każdej dystrybucji systemu operacyjnego z rodziny `GNU/Linux`, `MacOS` oraz `Windows`. Oprogramowanie dostarczane jest zwykle w postaci pojedynczego pliku, a importowane biblioteki są pobierane automatycznie.

Najłatwiejszą metodą budowy dokumentu jest użycie kompilatora `Typst` w trybie śledzenia zmian dokumentu:
```bash
typst watch main.typ
```

## Licencja

Niniejszy szablon dostępny jest na licencji `GNU LGPL v2.1`. Stosowanie, modyfikowanie i rozpowszechnianie niniejszego szablonu jest dozwolone w dowolnym celu, przy czym sam szablon traktowany jest jak zewnętrzna biblioteka.
