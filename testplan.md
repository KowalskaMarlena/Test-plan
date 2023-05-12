# Test plan dla rezerwacji miejsc w kinie

## Cel testu:

- Zweryfikować poprawność działania funkcji rezerwacji miejsc w kinie w aplikacji.

## Środowisko testowe:

- System operacyjny: Windows 10
- Przeglądarka: Google Chrome
- Dane testowe: zestaw przykładowych danych rezerwacji (poprawnych i niepoprawnych)

## Scenariusze testowe:

### A. Poprawna rezerwacja jednego miejsca w kinie jako zalogowany użytkownik.

Warunek wstępny: Użytkownik jest zalogowany i znajduje się na podtronie do wyboru miejsc.

- Krok 1: Wybierz pole oznaczone kolorem zielonym.
- Krok 2: Kliknij przycisk „Potwierdź rezerwacje”.

Oczekiwany rezultat: Użytkownik drogą mailowa otrzyma potwierdzenie rezerwacji wybranego miejsca z obowiązkiem zapłaty w kinie przed seansem.

### B. Poprawna rezerwacja kilku miejsc w kinie jako zalogowany użytkownik.

Warunek wstępny: Użytkownik jest zalogowany i znajduje się na podtronie do wyboru miejsc.

- Krok 1: Wybierz kilka pól oznaczonch kolorem zielonym.
- Krok 2: Kliknij przycisk „Potwierdź rezerwacje”.

Oczekiwany rezultat: Użytkownik drogą mailowa otrzyma potwierdzenie rezerwacji wybranych miejsc z obowiązkiem zapłaty w kinie przed seansem.

### C. Niepoprawna rezerwacja miejsc w kinie jako gość.

Warunek wstępny: Użytkownik nie jest zalogowany i znajduje się na podtronie do wyboru miejsc.

- Krok 1: Wybierz pole oznaczone kolorem zielonym.
- Krok 2: Kliknij przycisk „Potwierdź rezerwacje”

Oczekiwany wynik: Wyświetlony zostanie komunikat informujący, że użytkownik musi się zalogować lub jeśli nie posiada konta – zarejestrować.

### D. Niepoprawna rezerwacja zalogowanego użytkownika – wybór zarezerwowanego miejsca.

Warunek wstępny: Użytkownik jest zalogowany i znajduje się na podtronie do wyboru miejsc.

- Krok 1: Wybierz pole oznaczone kolorem czerwonym

Oczekiwany rezultat: Wyświetlony zostanie komunikat o braku możliwości rezerwacji wybranego miejsca.

### E. Niepoprawna rezerwacja z powodu braku wykonania akcji.

Warunek wstępny: Użytkownik znajduje się na podtronie do wyboru miejsc.

- Krok 1: Wybierz pole oznaczone kolorem zielonym.
- Krok 2: Nie wykonuj akcji „Potwierdź rezerwacje” przez 5 minut.

Oczekiwany rezultat: Gdy użytkownik przez 5 minut nie kliknie w pole „Potwierdź rezerwacje” zostaje przeniesiony do strony głównej aplikacji. Wyświetlony zostanie komunikat o niepowodzeniu dokonania rezerwacji wybranego miejsca.

## Procedury testowe:

- Przejdź przez każdy scenariusz testowy opisany powyżej.
- Zanotuj wyniki każdego kroku testowego, w tym oczekiwane i rzeczywiste rezultaty.
- W przypadku wystąpienia błędów, zapisz szczegółowe informacje o błędzie, takie jak komunikat o błędzie, kroki reprodukujące błąd, identyfikator błędu itp.

## Środki testowe:

- Komputer z zainstalowanym systemem operacyjnym i przeglądarką.
- Przykładowe miejsca do rezerwacji (poprawne i niepoprawne).

## Ryzyka i uwagi:

- Monitoruj czas odpowiedzi aplikacji, aby upewnić się, że rezerwacja jest wykonywane w odpowiednim czasie.

## Harmonogram testów:

- Etap 1: Przygotowanie środowiska testowego, konfiguracja danych testowych - 2 dni.
- Etap 2: Przeprowadzenie testów – 3 dni
- Etap 3: Analiza wyników, raportowanie defektów - 1 dzień.

## Raportowanie wyników:

- Wszystkie defekty zostaną zgłoszone i zarejestrowane w systemie zarządzania defektami, zawierając szczegółowe informacje o defekcie, kroki reprodukujące i oczekiwane działanie.
