# Test Case: Logowanie z niepoprawnym hasłem (OLX.pl)

**ID:** TC_OLX_LOGIN_002

**Opis** Weryfikacja obsługi błędu podczas próby logowania z poprawnym e-mailem, ale niepoprawnym hasłem.

**Kroki:**
Otwórz przeglądarkę i przejdź na stronę https://www.olx.pl.
Kliknij przycisk "Twoje konto" w prawym górnym rogu.
Wybierz opcję "Zaloguj się".
Wpisz adres e-mail w polu "E-mail".
Wpisz hasło w polu "Hasło".
Kliknij przycisk "Zaloguj się".

**Dane testowe:**
E-mail: test@example.com
Hasło: ZleHaslo456

**Oczekiwany wynik:** Wyświetlenie komunikatu błędu "Hasło jest nieprawidłowe" (lub podobny), użytkownik pozostaje na formularzu logowania, nie jest zalogowany.

**Rzeczywisty wynik:** Wyświetla się komunikat błędu "Hasło jest nieprawidłowe. Jeśli nie pamiętasz hasła, możesz je zresetować.", użytkownik pozostaje na formularzu, nie jest zalogowany.

**Status:** Zaliczony

**Screenshot:**
<img width="1918" height="1016" alt="Zrzut ekranu 2026-01-28 191827" src="https://github.com/user-attachments/assets/eee6861c-5bd3-41da-a83c-b65e563e3726" />
