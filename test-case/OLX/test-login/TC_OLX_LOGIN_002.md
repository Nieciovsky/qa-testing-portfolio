# Test Case: Logowanie z niepoprawnym hasłem (OLX.pl)

**ID:** TC_OLX_LOGIN_002

**Opis** \
Weryfikacja obsługi błędu podczas próby logowania z poprawnym e-mailem, ale niepoprawnym hasłem.

**Kroki:**\
1. Otwórz przeglądarkę i przejdź na stronę https://www.olx.pl.<br>
2. Kliknij przycisk "Twoje konto" w prawym górnym rogu.<br>
3. Wybierz opcję "Zaloguj się".<br>
4. Wpisz adres e-mail w polu "E-mail".<br>
5. Wpisz hasło w polu "Hasło".<br>
6. Kliknij przycisk "Zaloguj się".<br>

**Dane testowe:**<br>
E-mail: test@example.com<br>
Hasło: ZleHaslo456<br>

**Oczekiwany wynik:** \
Wyświetlenie komunikatu błędu "Hasło jest nieprawidłowe" (lub podobny), użytkownik pozostaje na formularzu logowania, nie jest zalogowany.

**Rzeczywisty wynik:** \
Wyświetla się komunikat błędu "Hasło jest nieprawidłowe. Jeśli nie pamiętasz hasła, możesz je zresetować.", użytkownik pozostaje na formularzu, nie jest zalogowany.

**Status:** Zaliczony

**Screenshot:**
<img width="1918" height="1016" alt="Zrzut ekranu 2026-01-28 191827" src="https://github.com/user-attachments/assets/eee6861c-5bd3-41da-a83c-b65e563e3726" />
