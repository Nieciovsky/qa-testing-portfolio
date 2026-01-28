# Test Case: Poprawne logowanie z ważnymi danymi (OLX.pl)

**ID:** TC_OLX_LOGIN_001

**Opis:** \
Weryfikacja, czy użytkownik może poprawnie zalogować się do konta OLX przy użyciu ważnych danych uwierzytelniających (e-mail i hasło).

**Kroki:** <br>
Otwórz przeglądarkę i przejdź na stronę https://www.olx.pl.<br>
Kliknij przycisk "Twoje konto" w prawym górnym rogu.<br>
Wybierz opcję "Zaloguj się".<br>
Wpisz adres e-mail w polu "E-mail".<br>
Wpisz hasło w polu "Hasło".<br>
Kliknij przycisk "Zaloguj się".<br>

**Dane testowe:**<br>
E-mail: test@example.com<br>
Hasło: PoprawneHaslo123!<br>

**Oczekiwany wynik:** Użytkownik zostaje zalogowany a strona przekierowuje do panelu "Moje OLX". Brak komunikatów błędów.

**Rzeczywisty wynik:** Użytkownik zostaje zalogowany a strona przekierowuje do panelu "Moje OLX". Brak komunikatów błędów.

**Status:** Zaliczony
