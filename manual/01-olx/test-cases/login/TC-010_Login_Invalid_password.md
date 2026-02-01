# TC-010 – Login attempt with correct email but invalid password

**Project:** OLX.pl  
**Module:** Authentication → Login form  
**Type:** Negative – Credential validation  
**Priority:** High  
**Preconditions:**  
- Valid email address known  
- Login page is open

**Test Data:**  
- Email: test@example.com  
- Password: ZleHaslo456 (incorrect)

**Steps to Reproduce:**
1. Navigate to https://www.olx.pl
2. Click "Twoje konto" in the top-right corner
3. Select "Zaloguj się"
4. Enter valid email in the "E-mail" field
5. Enter incorrect password in the "Hasło" field
6. Click "Zaloguj się"

**Expected Result:**
- Login is prevented
- Error message displayed, e.g. "Hasło jest nieprawidłowe. Jeśli nie pamiętasz hasła, możesz je zresetować."
- User remains on the login form

**Actual Result:**  
- Error message: "Hasło jest nieprawidłowe. Jeśli nie pamiętasz hasła, możesz je zresetować."
- Correct behavior – login blocked

**Status:** ✅ Passed  