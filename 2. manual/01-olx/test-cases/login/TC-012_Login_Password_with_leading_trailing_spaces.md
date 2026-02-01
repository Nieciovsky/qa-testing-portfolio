# TC-012 – Login attempt with password containing leading/trailing spaces (no trimming)

**Project:** OLX.pl  
**Module:** Authentication → Login form → Password sanitization  
**Type:** Negative – Input handling / Usability  
**Priority:** Medium  
**Preconditions:** Valid credentials known

**Test Data:**  
- Email: test@example.com  
- Password: " PoprawneHaslo123! " (with spaces)

**Steps to Reproduce:**
1. Navigate to login page
2. Enter valid email
3. Enter password with leading and trailing spaces
4. Click "Zaloguj się"

**Expected Result:**
- System trims whitespace automatically
- Successful login to "Moje OLX"
- No error messages

**Actual Result:**
- Error message: "Hasło jest nieprawidłowe. Jeśli nie pamiętasz hasła, możesz je zresetować."
- Login failed – spaces not trimmed

**Status:** ❌ Failed  
**Related Bug:** [BUG-002 – Password field does not trim leading/trailing spaces](../bug-reports/BUG-002_Password_field_does_not_trim_leading_trailing_spaces.md)

**Notes:** Common copy-paste issue (password managers, mobile keyboards). Contrast with TC-009 (email is trimmed).