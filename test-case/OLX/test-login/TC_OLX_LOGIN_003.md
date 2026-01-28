# Test Case: Logowanie z niepoprawnym adresem e-mail (OLX.pl)

**ID:** TC_OLX_LOGIN_003

**Opis:** \
Weryfikacja obsługi błędu podczas próby logowania z niepoprawnym e-mailem, ale poprawnym hasłem.

**Kroki:**\
1. Otwórz przeglądarkę i przejdź na stronę https://www.olx.pl. <br>
2. Kliknij przycisk "Twoje konto" w prawym górnym rogu. <br>
3. Wybierz opcję "Zaloguj się". <br>
4. Wpisz adres e-mail w polu "E-mail". <br>
5. Wpisz hasło w polu "Hasło". <br>
6. Kliknij przycisk "Zaloguj się". <br>
 
**Dane testowe:**\
E-mail: niepoprawnyemail@example.com <br>
Hasło: PoprawneHaslo123! <br>

**Oczekiwany wynik:** \
Wyświetlenie komunikatu błędu "E-mail jest nieprawidłowy" (lub podobny), użytkownik pozostaje na formularzu logowania, nie jest zalogowany.

**Rzeczywisty wynik:** \
Wyświetlenie komunikatu błędu "Coś poszło nie tak...", użytkownik pozostaje na formularzu logowania, nie jest zalogowany.

**Status:** Zaliczony

**Screenshot"**
<img width="1918" height="1020" alt="Zrzut ekranu 2026-01-28 192353" src="https://github.com/user-attachments/assets/1f1a02aa-58ad-450e-8cbe-4b4d903698e1" />
