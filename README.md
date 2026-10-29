# Dane do aplikacji Tracker obligacji skarbowych

Publiczne dane rynkowe dla hobbystycznej aplikacji iOS do śledzenia polskich detalicznych obligacji skarbowych.
Aplikacja pobiera stąd jeden plik, `bonds.json`: parametry serii obligacji, miesięczne odczyty inflacji,
historię stopy referencyjnej NBP i dni ustawowo wolne od pracy. Wszystkie obliczenia robi aplikacja lokalnie
na telefonie. Dane użytkownika nigdy tu nie trafiają.

Adres pliku: https://marcin0709.github.io/bond-tracker-data/bonds.json

## Źródła

- Parametry serii: listy emisyjne obligacji skarbowych, Ministerstwo Finansów (obligacjeskarbowe.pl).
- Inflacja: Główny Urząd Statystyczny (stat.gov.pl), wskaźniki cen towarów i usług konsumpcyjnych.
- Stopa referencyjna: Narodowy Bank Polski (static.nbp.pl).
- Dni wolne od pracy: Dziennik Ustaw (api.sejm.gov.pl).

Dane zostały przetworzone: przepisane do formatu `bonds.json`, stopy zapisane jako ułamek; przy każdym odczycie
inflacji jest data jego publikacji, a data pobrania jest w danych źródłowych. Pole `attribution` w pliku
powtarza te informacje.

## Zastrzeżenie

To projekt hobbystyczny, bez gwarancji poprawności i aktualności danych. Nie jest poradą finansową ani
inwestycyjną. Wiążące są zawsze listy emisyjne i informacje banku prowadzącego rejestr obligacji.

## Aktualizacja

Plik jest składany skryptami w prywatnym repozytorium aplikacji i na razie kopiowany tutaj ręcznie.
