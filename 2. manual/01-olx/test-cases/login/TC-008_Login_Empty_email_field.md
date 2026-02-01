# TC-008 – Login attempt with empty email field

**Project:** OLX.pl  
**Module:** Authentication → Login form → Required fields  
**Type:** Negative – Required field validation  
**Priority:** High  
**Preconditions:** Password entered

**Test Data:**  
- Email: (empty)  
- Password: PoprawneHaslo123!

**Steps to Reproduce:**
1. Navigate to login page
2. Leave "E-mail" field empty
3. Enter valid password
4. Click "Zaloguj się"

**Expected Result:**
- Login prevented
- Error message: "Wpisz swój e-mail" or similar required field indication
- Focus/highlight on email field (good UX)

**Actual Result:**  
- Message: "Wpisz swój e-mail"
- Correct blocking

**Status:** ✅ Passed  