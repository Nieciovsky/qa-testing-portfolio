# BUG-002 – Password field does not trim leading or trailing spaces

**Project:** OLX.pl  
**Module/Component:** Authentication → Login form  
**Bug type:** Usability / Input validation  
**Reported:** 2026-01-19  
**Related test case:** TC-OLX-LOGIN-012 (Negative – Password with extra spaces)

**Environment:**
- Browser: Chrome 131 (latest stable)
- OS: Windows 11
- Resolution: 1920×1080
- Device: Desktop
- User state: Logged out

**Steps to Reproduce:**
1. Navigate to https://www.olx.pl
2. Click "Twoje konto" (top right corner)
3. Select "Zaloguj się"
4. Enter a valid email address in the "E-mail" field
5. In the password field, enter a correct password with leading and/or trailing spaces, e.g. `" PoprawneHaslo123! "`
6. Click "Zaloguj się" or press Enter

**Actual Result:**
- Error message appears:  
  `"Hasło jest nieprawidłowe. Jeśli nie pamiętasz hasła, możesz je zresetować."`
- User remains on the login form (not logged in)

**Expected Result (industry best practice):**
- System automatically trims leading and trailing whitespace from the password field
- User is successfully logged in (no error shown)

**Severity:** Minor (Usability / Cosmetic) – does not prevent correct login, but causes unnecessary login failures for common copy-paste scenarios  
**Priority:** Medium / Low – improves user experience,

**Attachments:**
![BUG-002 – Login error with trailing spaces in password](https://github.com/user-attachments/assets/d3faac34-a96a-4b41-ad39-753ddb41eed4)