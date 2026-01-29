# Spis Treści | Test Cases – Logowanie OLX
## 1. Scenariusze pozytywne (Happy path)
1. [Logowanie poprawnym adresem e-mail i poprawnym hasłem](#TC_OLX_LOGIN_001)
2. [Logowanie po wcześniejszym wylogowaniu](#TC_OLX_LOGIN_002)
3. [Logowanie przy użyciu klawiatury (Enter zamiast kliknięcia przycisku)](#TC_OLX_LOGIN_003)
4. [Poprawne przekierowanie po zalogowaniu (dashboard / strona główna)](#TC_OLX_LOGIN_004)
## 2. Walidacja danych wejściowych – e-mail
5. [Logowanie z niepoprawnym formatem e-mail (brak @)](#TC_OLX_LOGIN_005)
6. [Logowanie z niepoprawnym formatem e-mail (brak domeny)](#TC_OLX_LOGIN_006)
7. [Logowanie z nieistniejącym adresem e-mail](#TC_OLX_LOGIN_007)
8. [Próba logowania bez podania adresu e-mail](#TC_OLX_LOGIN_008)
9. [Spacje przed / po adresie e-mail (trimowanie)](#TC_OLX_LOGIN_009)
## 3. Walidacja danych wejściowych – hasło
10. [Logowanie z niepoprawnym hasłem](#TC_OLX_LOGIN_010)
11. [Próba logowania bez podania hasła](#TC_OLX_LOGIN_011)
12. [Hasło z dodatkowymi spacjami (na początku / końcu)](#TC_OLX_LOGIN_012)
13. [Widoczność znaków hasła (maskowanie)](#TC_OLX_LOGIN_013)
## 4. Komunikaty błędów (UX / UI)
14. [Wyświetlenie komunikatu błędu przy niepoprawnych danych](#TC_OLX_LOGIN_014h)
15. [Czy komunikat błędu znika po poprawieniu danych](#TC_OLX_LOGIN_015)
## 5. Przycisk „Zaloguj” i elementy formularza
16. [Przycisk „Zaloguj” nieaktywny przy pustych polach](#TC_OLX_LOGIN_016)
17. [Przycisk „Zaloguj” aktywny po uzupełnieniu danych](#TC_OLX_LOGIN_017)
18. [Widoczność i dostępność linku „Nie pamiętam hasła”](#TC_OLX_LOGIN_018)

---



## 1. Scenariusze pozytywne (Happy path)

<h3 id="tc_olx_login_001"> 1.1 Logowanie poprawnym adresem e-mail i poprawnym hasłem </h3>

**ID:** TC_OLX_LOGIN_001

**Opis:** \
Weryfikacja, czy użytkownik może poprawnie zalogować się do konta OLX przy użyciu ważnych danych uwierzytelniających (e-mail i hasło).

**Kroki:** 
1. Otwórz przeglądarkę i przejdź na stronę https://www.olx.pl.<br>
2. Kliknij przycisk "Twoje konto" w prawym górnym rogu.<br>
3. Wybierz opcję "Zaloguj się".<br>
4. Wpisz adres e-mail w polu "E-mail".<br>
5. Wpisz hasło w polu "Hasło".<br>
6. Kliknij przycisk "Zaloguj się".<br>

**Dane testowe:**<br>
E-mail: test@example.com<br>
Hasło: PoprawneHaslo123!<br>

**Oczekiwany wynik:** \


Użytkownik zostaje zalogowany a strona przekierowuje do panelu "Moje OLX". Brak komunikatów błędów.

**Rzeczywisty wynik:** \
Użytkownik zostaje zalogowany a strona przekierowuje do panelu "Moje OLX". Brak komunikatów błędów.

**Status:** Zaliczony

---

<h3 id="tc_olx_login_002"> 1.2 Logowanie po wcześniejszym wylogowaniu </h3>

**ID:** TC_OLX_LOGIN_002

**Opis:** \
Weryfikacja, czy użytkownik może ponownie zalogować się do konta OLX po wcześniejszym wylogowaniu.

**Kroki:** 
1. Otwórz przeglądarkę i przejdź na stronę https://www.olx.pl 
2. Kliknij przycisk "Twoje konto" w prawym górnym rogu.
3. Wybierz opcję "Zaloguj się".
4. Wpisz adres e-mail w polu "E-mail".
5. Wpisz hasło w polu "Hasło".
6. Kliknij przycisk "Zaloguj się".
7. Po zalogowaniu, najedź kursorem na pole "Twoje konto" w prawym górnym rogu.
8. Wybierz opcję "Wyloguj się".
9. Powtórz kroki 2–6, aby zalogować się ponownie przy użyciu tych samych danych.


**Dane testowe:**<br>
E-mail: test@example.com<br>
Hasło: PoprawneHaslo123!<br>

**Oczekiwany wynik:** \
Użytkownik zostaje zalogowany po raz pierwszy, następnie wylogowany. Po ponownym zalogowaniu przy użyciu tych samych danych użytkownik ponownie zostaje przekierowany do panelu "Moje OLX". Brak komunikatów błędów.

**Rzeczywisty wynik:** \
Użytkownik zostaje zalogowany po raz pierwszy, następnie wylogowany. Po ponownym zalogowaniu przy użyciu tych samych danych użytkownik ponownie zostaje przekierowany do panelu "Moje OLX". Brak komunikatów błędów.

**Status:** Zaliczony

---

<h3 id="tc_olx_login_003"> 1.3 Logowanie po wcześniejszym wylogowaniu </h3>

**ID:** TC_OLX_LOGIN_003

**Opis:** \
Weryfikacja, czy użytkownik może zalogować się do konta OLX, używając klawisza Enter zamiast kliknięcia przycisku "Zaloguj się".

**Kroki:** 
1. Otwórz przeglądarkę i przejdź na stronę https://www.olx.pl 
2. Kliknij przycisk "Twoje konto" w prawym górnym rogu.
3. Wybierz opcję "Zaloguj się".
4. Wpisz adres e-mail w polu "E-mail".
5. Wpisz hasło w polu "Hasło".
6. Naciśnij klawisz Enter na klawiaturze zamiast kliknięcia przycisku "Zaloguj się"

**Dane testowe:**<br>
E-mail: test@example.com<br>
Hasło: PoprawneHaslo123!<br>

**Oczekiwany wynik:** \
Użytkownik zostaje zalogowany i przekierowany do panelu "Moje OLX". Brak komunikatów błędów.

**Rzeczywisty wynik:** \
Użytkownik zostaje zalogowany i przekierowany do panelu "Moje OLX". Brak komunikatów błędów.

**Status:** Zaliczony

---

<h3 id="tc_olx_login_004"> 1.4 Logowanie po wcześniejszym wylogowaniu </h3>

**ID:** TC_OLX_LOGIN_004

**Opis:** \
Weryfikacja, czy po zalogowaniu użytkownik jest poprawnie przekierowywany do panelu "Moje OLX" (dashboard) lub strony głównej konta.

**Kroki:** 
1. Otwórz przeglądarkę i przejdź na stronę https://www.olx.pl 
2. Kliknij przycisk "Twoje konto" w prawym górnym rogu.
3. Wybierz opcję "Zaloguj się".
4. Wpisz adres e-mail w polu "E-mail".
5. Wpisz hasło w polu "Hasło".
6. Kliknij przycisk "Zaloguj się".

**Dane testowe:**<br>
E-mail: test@example.com<br>
Hasło: PoprawneHaslo123!<br>

**Oczekiwany wynik:** \
Użytkownik zostaje zalogowany i automatycznie przekierowany do panelu "Moje OLX" lub strony głównej konta. Brak błędów lub niepoprawnych przekierowań.

**Rzeczywisty wynik:** \
Użytkownik zostaje zalogowany i automatycznie przekierowany do panelu "Moje OLX" lub strony głównej konta. Brak błędów lub niepoprawnych przekierowań.

**Status:** Zaliczony

---

## 2. Walidacja danych wejściowych – e-mail

<h3 id="tc_olx_login_005"> 2.1 Logowanie z niepoprawnym formatem e-mail (brak @) </h3>

**ID:** TC_OLX_LOGIN_005

**Opis:** \
Weryfikacja, czy system poprawnie reaguje na próbę logowania przy użyciu niepoprawnego formatu adresu e-mail (brak znaku "@").

**Kroki:** 
1. Otwórz przeglądarkę i przejdź na stronę https://www.olx.pl.<br>
2. Kliknij przycisk "Twoje konto" w prawym górnym rogu.<br>
3. Wybierz opcję "Zaloguj się".<br>
4. Wpisz adres e-mail w polu "E-mail".<br>
5. Wpisz hasło w polu "Hasło".<br>
6. Kliknij przycisk "Zaloguj się".<br>

**Dane testowe:**<br>
E-mail: testexample.com<br>
Hasło: PoprawneHaslo123!<br>

**Oczekiwany wynik:** \
System nie pozwala zalogować się i wyświetla komunikat błędu informujący o niepoprawnym formacie adresu e-mail.

**Rzeczywisty wynik:** \
System nie pozwala zalogować się i wyświetla komunikat błędu "To nie wygląda jak adres mailowy..." informujący o niepoprawnym formacie adresu e-mail.

**Status:** Zaliczony

---

<h3 id="tc_olx_login_006"> 2.2 Logowanie z niepoprawnym formatem e-mail (brak domeny) </h3>

**ID:** TC_OLX_LOGIN_006

**Opis:** \
Weryfikacja, czy system poprawnie reaguje na próbę logowania przy użyciu adresu e-mail bez domeny (np. "test@").

**Kroki:** 
1. Otwórz przeglądarkę i przejdź na stronę https://www.olx.pl.<br>
2. Kliknij przycisk "Twoje konto" w prawym górnym rogu.<br>
3. Wybierz opcję "Zaloguj się".<br>
4. Wpisz adres e-mail w polu "E-mail".<br>
5. Wpisz hasło w polu "Hasło".<br>
6. Kliknij przycisk "Zaloguj się".<br>

**Dane testowe:**<br>
E-mail: test@<br>
Hasło: PoprawneHaslo123!<br>

**Oczekiwany wynik:** \
System nie pozwala zalogować się i wyświetla komunikat błędu informujący o niepoprawnym formacie adresu e-mail.

**Rzeczywisty wynik:** \
System nie pozwala zalogować się i wyświetla komunikat błędu "To nie wygląda jak adres mailowy..." informujący o niepoprawnym formacie adresu e-mail.

**Status:** Zaliczony

---

<h3 id="tc_olx_login_007"> 2.3 Logowanie z nieistniejącym adresem e-mail </h3>

**ID:** TC_OLX_LOGIN_007

**Opis:** \
Weryfikacja, czy system poprawnie reaguje na próbę logowania przy użyciu adresu e-mail, który nie istnieje w systemie OLX.

**Kroki:**
1. Otwórz przeglądarkę i przejdź na stronę https://www.olx.pl. <br>
2. Kliknij przycisk "Twoje konto" w prawym górnym rogu. <br>
3. Wybierz opcję "Zaloguj się". <br>
4. Wpisz adres e-mail w polu "E-mail". <br>
5. Wpisz hasło w polu "Hasło". <br>
6. Kliknij przycisk "Zaloguj się". <br>
 
**Dane testowe:** \
E-mail: nieistniejący@example.com <br>
Hasło: PoprawneHaslo123! <br>

**Oczekiwany wynik:** \
Wyświetlenie komunikatu błędu "E-mail jest nieprawidłowy" (lub podobny), użytkownik pozostaje na formularzu logowania, nie jest zalogowany.

**Rzeczywisty wynik:** \
Wyświetlenie komunikatu błędu "Coś poszło nie tak...", użytkownik pozostaje na formularzu logowania, nie jest zalogowany.

**Status:** Zaliczony

---

<h3 id="tc_olx_login_008"> 2.4 Logowanie z nieistniejącym adresem e-mail </h3>

**ID:** TC_OLX_LOGIN_008

**Opis:** \
Weryfikacja, czy system poprawnie reaguje na próbę logowania, gdy użytkownik nie wprowadzi adresu e-mail.

**Kroki:**
1. Otwórz przeglądarkę i przejdź na stronę https://www.olx.pl. <br>
2. Kliknij przycisk "Twoje konto" w prawym górnym rogu. <br>
3. Wybierz opcję "Zaloguj się". <br>
4. Pole "E-mail" pozostaw puste. <br>
5. Wpisz hasło w polu "Hasło". <br>
6. Kliknij przycisk "Zaloguj się". <br>
 
**Dane testowe:** \
E-mail: *(puste pole)* <br>
Hasło: PoprawneHaslo123! <br>

**Oczekiwany wynik:** \
System nie pozwala zalogować się i wyświetla komunikat błędu informujący o konieczności wprowadzenia adresu e-mail.

**Rzeczywisty wynik:** \
System nie pozwala zalogować się i wyświetla komunikat błędu "Wpisz swój e-mail" informujący o konieczności wprowadzenia adresu e-mail.

**Status:** Zaliczony

---

<h3 id="tc_olx_login_009"> 2.5 Spacje przed / po adresie e-mail (trimowanie) </h3>

**ID:** TC_OLX_LOGIN_009

**Opis:** \
Weryfikacja, czy system poprawnie obsługuje adres e-mail z dodatkowymi spacjami przed lub po wprowadzonej wartości (czy system je automatycznie usuwa – trimuje).

**Kroki:**
1. Otwórz przeglądarkę i przejdź na stronę https://www.olx.pl. <br>
2. Kliknij przycisk "Twoje konto" w prawym górnym rogu. <br>
3. Wybierz opcję "Zaloguj się". <br>
4. Wpisz adres e-mail z dodatkowymi spacjami przed i po (np. " test@example.com ").
5. Wpisz hasło w polu "Hasło". <br>
6. Kliknij przycisk "Zaloguj się". <br>
 
**Dane testowe:** \
E-mail: `" test@example.com "` <br>
Hasło: PoprawneHaslo123! <br>

**Oczekiwany wynik:** \
System usuwa nadmiarowe spacje i pozwala użytkownikowi zalogować się do konta OLX. Brak komunikatów błędów.

**Rzeczywisty wynik:** \
System usuwa nadmiarowe spacje i pozwala użytkownikowi zalogować się do konta OLX. Brak komunikatów błędów.

**Status:** Zaliczony

---

## 3. Walidacja danych wejściowych – hasło

<h3 id="tc_olx_login_010"> 3.1 Logowanie z niepoprawnym hasłem </h3>

**ID:** TC_OLX_LOGIN_010

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

---

<h3 id="tc_olx_login_011"> 3.2 Próba logowania bez podania hasła</h3>

**ID:** TC_OLX_LOGIN_011


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
Wyświetlenie komunikatu błędu pod polem "Hasło": "Masz pewność co do hasła? Jest zbyt krótkie", użytkownik pozostaje na formularzu logowania, przycisk "Zaloguj się" nieaktywny. Użytkownik pozostaje niezalogowany.

**Status:** Zaliczony

---

<h3 id="tc_olx_login_012"> 3.3 Hasło z dodatkowymi spacjami (na początku / końcu) </h3>

**ID:** TC_OLX_LOGIN_012

**Opis** \
Weryfikacja, czy system poprawnie obsługuje hasło z dodatkowymi spacjami przed lub po wprowadzonej wartości (czy system je automatycznie usuwa – trimuje).

**Kroki:**
1. Otwórz przeglądarkę i przejdź na stronę https://www.olx.pl.<br>
2. Kliknij przycisk "Twoje konto" w prawym górnym rogu.<br>
3. Wybierz opcję "Zaloguj się".<br>
4. Wpisz adres e-mail w polu "E-mail".<br>
5. Wpisz hasło z dodatkowymi spacjami przed i po.
6. Kliknij przycisk "Zaloguj się".<br>

**Dane testowe:**<br>
E-mail: test@example.com<br>
Hasło: `" PoprawneHaslo123! "`

**Oczekiwany wynik:** \
System usuwa nadmiarowe spacje i pozwala użytkownikowi zalogować się do konta OLX. Brak komunikatów błędów.

**Rzeczywisty wynik:** \
Wyświetla się komunikat błędu "Hasło jest nieprawidłowe. Jeśli nie pamiętasz hasła, możesz je zresetować.", użytkownik pozostaje na formularzu, nie jest zalogowany.

**Status:** Niezaliczony

---

<h3 id="tc_olx_login_013"> 3.4 Hasło z dodatkowymi spacjami (na początku / końcu) </h3>

**ID:** TC_OLX_LOGIN_013

**Opis** \
Weryfikacja, czy znaki wpisywanego hasła są poprawnie maskowane (ukryte) w polu "Hasło" podczas logowania, aby chronić dane użytkownika.

**Kroki:**
1. Otwórz przeglądarkę i przejdź na stronę https://www.olx.pl.<br>
2. Kliknij przycisk "Twoje konto" w prawym górnym rogu.<br>
3. Wybierz opcję "Zaloguj się".<br>
4. Wpisz hasło w polu "Hasło"
5. Sprawdź, czy wpisywane znaki są wyświetlane jako kropki lub gwiazdki (maskowane).

**Dane testowe:**<br>
Hasło: `" PoprawneHaslo123! "`

**Oczekiwany wynik:** \
Wpisywane znaki hasła są maskowane (ukryte), np. jako kropki lub gwiazdki. Brak widocznych liter hasła na ekranie.

**Rzeczywisty wynik:** \
Wpisywane znaki hasła są maskowane (ukryte) jako kropki. Brak widocznych liter hasła na ekranie.

**Status:** Zaliczony

---

## 4.Komunikaty błędów (UX / UI)

<h3 id="tc_olx_login_014"> 4.1 Wyświetlenie komunikatu błędu przy niepoprawnych danych </h3>

**ID:** TC_OLX_LOGIN_014

**Opis** \
Weryfikacja, czy system wyświetla odpowiedni komunikat błędu, gdy użytkownik próbuje zalogować się przy użyciu niepoprawnego adresu e-mail lub hasła.

**Kroki:**\
1. Otwórz przeglądarkę i przejdź na stronę https://www.olx.pl.<br>
2. Kliknij przycisk "Twoje konto" w prawym górnym rogu.<br>
3. Wybierz opcję "Zaloguj się".<br>
4. Wpisz niepoprawny adres e-mail lub hasło w odpowiednich polach.
5. Kliknij przycisk "Zaloguj się".<br>
6. Zwróć uwagę na wyświetlony komunikat błędu.

**Dane testowe:**<br>
E-mail: test@example.com<br>
Hasło: ZleHaslo456<br>

**Oczekiwany wynik:** \
System wyświetla komunikat błędu informujący, że podane dane są nieprawidłowe i logowanie nie powiodło się. Komunikat jest czytelny i widoczny dla użytkownika.

**Rzeczywisty wynik:** \
System pod odpowiednim polem wyświetla komunikat błędu informujący, że podane dane są nieprawidłowe i logowanie nie powiodło się. Komunikat jest czytelny i widoczny dla użytkownika.

**Status:** Zaliczony

---

<h3 id="tc_olx_login_015"> 4.2 Czy komunikat błędu znika po poprawieniu danych </h3>

**ID:** TC_OLX_LOGIN_015

**Opis** \
Weryfikacja, czy komunikat błędu dotyczący niepoprawnych danych znika po wprowadzeniu poprawnego adresu e-mail i hasła oraz próbie ponownego zalogowania.

**Kroki:**\
1. Otwórz przeglądarkę i przejdź na stronę https://www.olx.pl.<br>
2. Kliknij przycisk "Twoje konto" w prawym górnym rogu.<br>
3. Wybierz opcję "Zaloguj się".<br>
4. Wpisz niepoprawny adres e-mail lub hasło w odpowiednich polach.
5. Zauważ wyświetlony komunikat błędu.
6. Wpisz poprawny adres e-mail i hasło.
7. Kliknij ponownie przycisk "Zaloguj się".

**Dane testowe:**<br>
E-mail: test@example.com<br>
Hasło: PoprawneHaslo123!<br>

**Oczekiwany wynik:** \
Po poprawnym wprowadzeniu danych komunikat błędu znika, a użytkownik zostaje zalogowany i przekierowany do panelu "Moje OLX".

**Rzeczywisty wynik:** \
Po poprawnym wprowadzeniu danych komunikat błędu znika, a użytkownik zostaje zalogowany i przekierowany do panelu "Moje OLX".

**Status:** Zaliczony

---

## 5.Komunikaty błędów (UX / UI)

<h3 id="tc_olx_login_016"> 5.1 Przycisk „Zaloguj” nieaktywny przy pustych polach </h3>

**ID:** TC_OLX_LOGIN_016

**Opis** \
Weryfikacja, czy przycisk "Zaloguj" jest nieaktywny (disabled), gdy pola "E-mail" i "Hasło" są puste, aby zapobiec wysyłaniu formularza z brakującymi danymi.

**Kroki:**\
1. Otwórz przeglądarkę i przejdź na stronę https://www.olx.pl.<br>
2. Kliknij przycisk "Twoje konto" w prawym górnym rogu.<br>
3. Wybierz opcję "Zaloguj się".<br>
4. Sprawdź stan przycisku "Zaloguj" przy:
    - obu pustych polach
    - pustym polu "E-mail" i wypełnionym polu "Hasło"
    - wypełnionym polu "E-mail" i pustym polu "Hasło"

**Dane testowe:**<br>
E-mail: *(puste pole)* <br>
Hasło: *(puste pole)* <br>

**Oczekiwany wynik:** \
Przycisk "Zaloguj" jest nieaktywny (nieklikalny) dopóki oba pola nie zostaną wypełnione poprawnymi danymi.

**Rzeczywisty wynik:** \
Przycisk "Zaloguj" jest nieaktywny (nieklikalny) dopóki oba pola nie zostaną wypełnione poprawnymi danymi.

**Status:** Zaliczony

---

<h3 id="tc_olx_login_01"> 5.2 Przycisk „Zaloguj” aktywny po uzupełnieniu danych </h3>

**ID:** TC_OLX_LOGIN_017

**Opis** \
Weryfikacja, czy przycisk "Zaloguj" staje się aktywny (klikany) po wprowadzeniu poprawnych danych w polach "E-mail" i "Hasło".

**Kroki:**\
1. Otwórz przeglądarkę i przejdź na stronę https://www.olx.pl.<br>
2. Kliknij przycisk "Twoje konto" w prawym górnym rogu.<br>
3. Wybierz opcję "Zaloguj się".<br>
4. Wpisz poprawny adres e-mail w polu "E-mail".
5. Wpisz poprawne hasło w polu "Hasło".
6. Sprawdź, czy przycisk "Zaloguj" zmieni stan na aktywny i jest klikalny.

**Dane testowe:**
E-mail: test@example.com <br>
Hasło: PoprawneHaslo123! <br>

**Oczekiwany wynik:** \
Po wprowadzeniu poprawnych danych przycisk "Zaloguj" staje się aktywny i pozwala użytkownikowi zalogować się do konta OLX.

**Rzeczywisty wynik:** \
Po wprowadzeniu poprawnych danych przycisk "Zaloguj" staje się aktywny i pozwala użytkownikowi zalogować się do konta OLX.

**Status:** Zaliczony

---

<h3 id="tc_olx_login_08"> 5.3 Widoczność i dostępność linku „Nie pamiętam hasła” </h3>

**ID:** TC_OLX_LOGIN_018

**Opis** \
Weryfikacja, czy link „Nie pamiętam hasła” jest widoczny i dostępny dla użytkownika oraz czy umożliwia przejście do procesu resetowania hasła.

**Kroki:**\
1. Otwórz przeglądarkę i przejdź na stronę https://www.olx.pl.<br>
2. Kliknij przycisk "Twoje konto" w prawym górnym rogu.<br>
3. Wybierz opcję "Zaloguj się".<br>
4. Zlokalizuj link „Nie pamiętam hasła” w formularzu logowania.
5. Kliknij link „Nie pamiętam hasła”.
6. Sprawdź, czy następuje przekierowanie do strony resetowania hasła.

**Dane testowe:** <br>
Brak danych testowych – weryfikacja widoczności i działania linku.

**Oczekiwany wynik:** \
Link „Nie pamiętam hasła” jest wyraźnie widoczny, dostępny (klikany) i po kliknięciu przenosi użytkownika do formularza resetowania hasła.

**Rzeczywisty wynik:** \
Link „Nie pamiętam hasła” jest wyraźnie widoczny, dostępny (klikany) i po kliknięciu przenosi użytkownika do formularza resetowania hasła.

**Status:** Zaliczony
