# Test plan dodania produktu do koszyka na podstawie API

## Cel testu

- Zweryfikowanie poprawności funkcjonalności dodawania produktu do koszyka z punktu widzenia żądania (request) i odpowiedzi (response).
- Upewnienie się, że żądanie i odpowiedź są zgodne z oczekiwaniami i spełniają wymagania.
- Sprawdzenie, czy interakcja między żądaniem a odpowiedzią przebiega prawidłowo.

## Zakres testu:

- Testowanie procesu dodawania produktu do koszyka.
- Weryfikacja poprawności danych przekazywanych w żądaniu i odpowiedzi.
- Testowanie różnych przypadków, takich jak dodawanie pojedynczego produktu, dodawanie produktów różnych typów, dodawanie produktu, który jest już w koszyku itp.

## Środowisko testowe:

- System operacyjny: Windows 10
- Przeglądarka internetowa: Google Chrome
- Narzędzia do testowania API lub narzędzia do testowania żądań i odpowiedzi HTTP
- Dane testowe: dostępne produkty testowe

## Ograniczenia:

- Testowanie zostanie przeprowadzone na wyznaczonym środowisku testowym.

## Scenariusze testowe:

### A. Dodawanie produktu do koszyka:

Warunki wstępne: Koszyk jest pusty. Strona lub interfejs API dodawania produktu do koszyka jest dostępny.

- Krok 1: Wykonaj żądanie HTTP dodania produktu do koszyka.
- Krok 2: Sprawdź poprawność żądania i odpowiedzi HTTP.
- Krok 3: Zweryfikuj, czy produkt został poprawnie dodany do koszyka.
- Krok 4: Sprawdź, czy wyświetlane dane produktu w koszyku są zgodne z oczekiwaniami.

## Procedury testowe:

### A. Dodawanie produktu do koszyka:

- Wykonaj żądanie HTTP dodania produktu do koszyka.
- Sprawdź, czy żądanie zawiera poprawne dane, takie jak identyfikator produktu, ilość itp.
- Zweryfikuj odpowiedź HTTP, sprawdzając kod odpowiedzi, treść odpowiedzi i inne pola odpowiedzi.
- Sprawdź, czy produkt został poprawnie dodany do koszyka.
- Sprawdź, czy wyświetlane dane produktu w koszyku są zgodne z oczekiwaniami.

## Kryteria sukcesu:

- Żądanie dodania produktu do koszyka zwraca prawidłową odpowiedź HTTP.
- Produkt zostaje poprawnie dodany do koszyka.
- Wyświetlane dane produktu w koszyku są zgodne z oczekiwaniami.

## Harmonogram testów:

- Przygotowanie środowiska testowego i danych testowych - 1 dzień.
- Przeprowadzenie testów dodawania produktu do koszyka z punktu widzenia żądania i odpowiedzi - 3 dni.
- Analiza wyników, raportowanie defektów - 1 dzień.

## Zasoby testowe:

- Zespół testujący, w tym testerzy i programiści.
- Środowisko testowe z wymaganymi konfiguracjami sprzętowymi i oprogramowaniem.
- Dostęp do danych testowych, w tym produktów testowych, identyfikatorów itp.

## Ryzyka i uwagi:

- Ryzyko: Nieprawidłowa komunikacja między żądaniem a odpowiedzią, co może prowadzić do błędów w procesie dodawania produktu do koszyka.
- Uwaga: Upewnij się, że testy obejmują różne przypadki, takie jak dodawanie produktów różnych typów, dodawanie produktu, który jest już w koszyku, itp.

## Raportowanie wyników:

- Wszystkie defekty zostaną zgłoszone i zarejestrowane w systemie zarządzania defektami, zawierając szczegółowe informacje o defekcie, kroki reprodukujące i oczekiwane działanie.
