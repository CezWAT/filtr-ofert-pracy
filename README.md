# filtr-ofert-pracy
Skrypty JavaScript do Greasemonkey/Tampermonkey ułatwiające przeglądanie ofert pracy w popularnych serwisach. Ukrywanie wybranych pracodawców i oznaczanie ofert według lokalizacji oraz trybu pracy.

## Problem: 

Ręczne odfiltrowywanie niepożądanych pracodawców i sprawdzanie lokalizacji każdej oferty.

## Funkcje: 

Ukrywanie firm z czarnej listy oraz oznaczanie ofert kolorową ramką zgodnie z regułą:
- zdalnie — zielona ramka;
- lokalizacja zgodna z wartością CITY i stacjonarnym lub hybrydowym lub zdalnym trybem pracy — zielona ramka;
- pozostałe przypadki — czerwona ramka.

## Konfiguracja: 
- firmy do czarnej listy dodaje się edytując plik i zmieniając wartość zmiennej w skrypcie "portal - czarna lista firm"

```
const blacklist = [
        'firma1',
        'firma2',
        'firma3'
    ];
```
  
- kolorowanie ramki wokół ogłoszenia ustawia się edytując wartość zmiennej w skrypcie "portal - ramki ofert według lokalizacji"

```const CITY = 'miasto';```

## Instalacja i użycie:

Wymagane rozszerzenie przeglądarki Greasemonkey/Tampermonkey lub podobne. 

## Ograniczenia:

Zmiany HTML na portalach mogą wymagać aktualizacji selektorów; kolor ramki jest wynikiem reguł skryptu, a nie gwarancją faktycznych warunków pracy.
