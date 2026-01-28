# Test Case: Poprawne logowanie z ważnymi danymi (OLX.pl)

**ID:** TC_OLX_LOGIN_001

**Opis:** \
Weryfikacja, czy użytkownik może poprawnie zalogować się do konta OLX przy użyciu ważnych danych uwierzytelniających (e-mail i hasło).

**Kroki:** <br>
1. Otwórz przeglądarkę i przejdź na stronę https://www.olx.pl.<br>
2. Kliknij przycisk "Twoje konto" w prawym górnym rogu.<br>
3. Wybierz opcję "Zaloguj się".<br>
4. Wpisz adres e-mail w polu "E-mail".<br>
5. Wpisz hasło w polu "Hasło".<br>
6. Kliknij przycisk "Zaloguj się".<br>

**Dane testowe:**<br>
E-mail: test@example.com<br>
Hasło: PoprawneHaslo123!<br>

**Oczekiwany wynik:** \ Użytkownik zostaje zalogowany a strona przekierowuje do panelu "Moje OLX". Brak komunikatów błędów.

**Rzeczywisty wynik:** \ Użytkownik zostaje zalogowany a strona przekierowuje do panelu "Moje OLX". Brak komunikatów błędów.

**Status:** Zaliczony
