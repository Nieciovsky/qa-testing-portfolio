# TC-011 – Login attempt with empty password field

**Project:** OLX.pl  
**Module:** Authentication → Login form → Required fields  
**Type:** Negative – Required field validation  
**Priority:** High  
**Preconditions:**  
- Valid email entered  
- Login page open

**Test Data:**  
- Email: test@example.com  
- Password: (empty)

**Steps to Reproduce:**
1. Navigate to login page (steps 1–4 from TC-010)
2. Leave "Hasło" field empty
3. Click "Zaloguj się"

**Expected Result:**
- Login prevented
- Error message under password field, e.g. "Masz pewność co do hasła? Jest zbyt krótkie" or "Proszę podać hasło"
- Submit button may be disabled or form highlighted

**Actual Result:**  
- Message: "Masz pewność co do hasła? Jest zbyt krótkie"  
- Button inactive / login blocked  
- Correct client-side validation

**Status:** ✅ Passed  
