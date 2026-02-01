# TC-006 – Login with invalid email format (no domain after @)

**Project:** OLX.pl  
**Module:** Authentication → Login form → Email validation  
**Type:** Negative – Input validation  
**Priority:** High  
**Preconditions:** Login page open

**Test Data:**  
- Email: test@  
- Password: PoprawneHaslo123!

**Steps to Reproduce:**
1. Navigate to login page (as in TC-005 steps 1–3)
2. Enter invalid email (no domain) in "E-mail"
3. Enter valid password
4. Click "Zaloguj się"

**Expected Result:**
- Login prevented
- Error message about invalid email format (e.g. "To nie wygląda jak adres mailowy...")

**Actual Result:**  
- Error message displayed correctly
- No login attempt processed

**Status:** ✅ Passed  
