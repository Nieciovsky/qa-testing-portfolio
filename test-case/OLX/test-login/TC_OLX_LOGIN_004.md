# Test Case: Próba logowania bez podania hasła (OLX.pl)

**ID:** TC_OLX_LOGIN_004

**Opis** \
Weryfikacja obsługi błędu podczas próby logowania bez podania hasła.

**Kroki:**
1. Otwórz przeglądarkę i przejdź na stronę https://www.olx.pl.<br>
2. Kliknij przycisk "Twoje konto" w prawym górnym rogu.<br>
3. Wybierz opcję "Zaloguj się".<br>
4. Wpisz adres e-mail w polu "E-mail".<br>
5. Pole "Hasło" pozostaw puste.<br>
6. Kliknij przycisk "Zaloguj się".<br>

**Dane testowe:**<br>
E-mail: test@example.com<br>
Hasło:<br>

**Oczekiwany wynik:** \
Wyświetlenie komunikatu błędu "Proszę podać hasło" (lub podobny), użytkownik pozostaje na formularzu logowania, nie jest zalogowany.

**Rzeczywisty wynik:** \
Wyświetlenie komunikatu błędu pod polem "Hasło": "Masz pewność co do hasła? Jest zbyt krótkie", użytkownik pozostaje na formularzu logowania, przycisk "Zaloguj się" nieaktywny. Urzytkownik pozostaje niezalogowany.

**Status:** Zaliczony

**Screenshot"**
<img width="1918" height="1018" alt="Zrzut ekranu 2026-01-28 193007" src="https://github.com/user-attachments/assets/17620f36-1c2c-41ac-b153-897d62edde39" />
