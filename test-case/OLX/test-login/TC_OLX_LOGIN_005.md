# Test Case: Próba logowania bez podania adresu e-mail (OLX.pl)

## **ID:** TC_OLX_LOGIN_005

#### **Opis** \
Weryfikacja obsługi błędu podczas próby logowania bez podania adresu e-mail.

### **Kroki:**
1. Otwórz przeglądarkę i przejdź na stronę https://www.olx.pl. <br>
2. Kliknij przycisk "Twoje konto" w prawym górnym rogu. <br>
3. Wybierz opcję "Zaloguj się". <br>
4. Pole "E-mail" pozostaw puste. <br>
5. Wpisz hasło w polu "Hasło". <br>
6. Kliknij przycisk "Zaloguj się". <br>

**Dane testowe:** <br>
E-mail: <br>
Hasło: DobreHasło <br>

**Oczekiwany wynik:** \
Wyświetlenie komunikatu błędu "Proszę wpisać adres e-mail" (lub podobny), użytkownik pozostaje na formularzu logowania, nie jest zalogowany.

**Rzeczywisty wynik:** \
Wyświetlenie komunikatu błędu pod polem "E-mail": "Wpisz swój e-mail", użytkownik pozostaje na formularzu logowania, przycisk "Zaloguj się" nieaktywny. Urzytkownik pozostaje niezalogowany.

**Status:** Zaliczony

**Screenshot"**
<img width="1918" height="1018" alt="Zrzut ekranu 2026-01-28 193007" src="https://github.com/user-attachments/assets/9cdaa61a-35be-47ca-a92b-65a4c06f182d" />
