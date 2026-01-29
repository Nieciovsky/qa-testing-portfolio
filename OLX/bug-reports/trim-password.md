# Bug Report: <br> Nieprawidłowa obsługa hasła z dodatkowymi spacjami – OLX.pl

**Tytuł:** System nie akceptuje hasła z dodatkowymi spacjami na początku lub końcu pola

**Data zgłoszenia:** 19 stycznia 2026
**ID testu powiązanego:** TC_OLX_LOGIN_012

**Środowisko:**
- Przeglądarka: Chrome 131 (najnowsza wersja)
- System: Windows 11
- Rozdzielczość: 1920×1080
- Urządzenie: Desktop
- Konto: Niezalogowany

**Kroki do powtórzenia:**
1. Otwórz przeglądarkę i przejdź na stronę https://www.olx.pl
2. Kliknij przycisk „Twoje konto” w prawym górnym rogu.
3. Wybierz opcję „Zaloguj się”.
4. Wpisz poprawny adres e-mail w polu „E-mail”.
5. Wpisz hasło z dodatkowymi spacjami na początku i końcu, np. ```" PoprawneHaslo123! "```.
6. Kliknij przycisk „Zaloguj się” lub naciśnij Enter.


**Oczekiwany rezultat:**  
System automatycznie usuwa nadmiarowe spacje (trimuje) i pozwala użytkownikowi zalogować się do konta OLX. Brak komunikatów błędów.

**Rzeczywisty rezultat:**  
Wyświetla się komunikat błędu: ```"Hasło jest nieprawidłowe. Jeśli nie pamiętasz hasła, możesz je zresetować."```
Użytkownik pozostaje na formularzu, nie jest zalogowany.


**Dodatkowe informacje:**
- **Priorytet:** Wysoki
- **Severity:** Major (blokuje logowanie przy standardowych zachowaniach użytkownika)
- **Zrzut ekranu:**  

<img width="1918" height="1020" alt="Zrzut ekranu 2026-01-29 125303" src="https://github.com/user-attachments/assets/d3faac34-a96a-4b41-ad39-753ddb41eed4" />

