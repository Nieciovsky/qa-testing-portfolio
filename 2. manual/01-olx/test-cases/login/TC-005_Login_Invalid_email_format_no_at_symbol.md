# TC-005 – Login with invalid email format (no @ symbol)

**Project:** OLX.pl  
**Module:** Authentication → Login form → Email validation  
**Type:** Negative – Input validation  
**Priority:** High  
**Preconditions:**  
- Login page is open  
- Valid password is ready

**Test Data:**  
- Email: testexample.com  
- Password: PoprawneHaslo123!

**Steps to Reproduce:**
1. Navigate to https://www.olx.pl
2. Click "Twoje konto" in the top-right corner
3. Select "Zaloguj się"
4. Enter invalid email (without @) in the "E-mail" field
5. Enter valid password in the "Hasło" field
6. Click "Zaloguj się"

**Expected Result:**
- System prevents login
- Error message is displayed, e.g. "To nie wygląda jak adres mailowy..." or similar validation feedback
- User remains on the login form

**Actual Result:** [Same as expected – success]

**Status:** ✅ Passed  
