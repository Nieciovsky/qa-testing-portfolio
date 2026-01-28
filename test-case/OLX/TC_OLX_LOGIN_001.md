# Test Case: Poprawne logowanie z ważnymi danymi (OLX.pl)

**ID:** TC_OLX_LOGIN_001

**Opis** Weryfikacja, czy użytkownik może poprawnie zalogować się do konta OLX przy użyciu ważnych danych uwierzytelniających (e-mail i hasło).

**Kroki:**
Otwórz przeglądarkę i przejdź na stronę https://www.olx.pl.
Kliknij przycisk "Twoje konto" w prawym górnym rogu.
Wybierz opcję "Zaloguj się".
Wpisz adres e-mail w polu "E-mail".
Wpisz hasło w polu "Hasło".
Kliknij przycisk "Zaloguj się".

**Dane testowe:**
E-mail: test@example.com
Hasło: PoprawneHaslo123!

**Oczekiwany wynik:** Użytkownik zostaje zalogowany a strona przekierowuje do panelu "Moje OLX". Brak komunikatów błędów.

**Rzeczywisty wynik:** Użytkownik zostaje zalogowany a strona przekierowuje do panelu "Moje OLX". Brak komunikatów błędów.

**Status:** Zaliczony
