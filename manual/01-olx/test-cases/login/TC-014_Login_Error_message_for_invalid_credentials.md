# TC-014 – Error message displayed for invalid login credentials

**Project:** OLX.pl  
**Module:** Authentication → Login form → Error handling / UX  
**Type:** Negative – Error messaging  
**Priority:** High  
**Preconditions:**  
- Login page is open  
- Valid credentials are known for comparison

**Test Data (invalid):**  
- Email: test@example.com  
- Password: ZleHaslo456 (incorrect)

**Steps to Reproduce:**
1. Navigate to https://www.olx.pl
2. Click "Twoje konto" in the top-right corner
3. Select "Zaloguj się"
4. Enter invalid email or password (or both)
5. Click "Zaloguj się"
6. Observe the displayed error message(s)

**Expected Result:**
- Clear, visible error message appears (e.g. "Hasło jest nieprawidłowe. Jeśli nie pamiętasz hasła, możesz je zresetować.")
- Message is associated with the incorrect field(s) or shown centrally
- Message is readable, properly styled (contrast, font size)
- User remains on the login form

**Actual Result:** 
- Error message displayed under the relevant field / form  
- Text: "Hasło jest nieprawidłowe. Jeśli nie pamiętasz hasła, możesz je zresetować."  
- Message is clear and visible  
- Correct UX behavior

**Status:** ✅ Passed  
