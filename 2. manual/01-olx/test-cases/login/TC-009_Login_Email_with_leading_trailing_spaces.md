# TC-009 – Login with email containing leading/trailing spaces (trim handling)

**Project:** OLX.pl  
**Module:** Authentication → Login form → Input sanitization  
**Type:** Positive – Usability / Trim behavior  
**Priority:** Medium  
**Preconditions:** Valid credentials known

**Test Data:**  
- Email: " test@example.com " (with spaces)  
- Password: PoprawneHaslo123!

**Steps to Reproduce:**
1. Navigate to login page
2. Enter email with extra spaces before/after
3. Enter valid password
4. Click "Zaloguj się"

**Expected Result:**
- System trims whitespace automatically
- Successful login and redirect to "Moje OLX"
- No error messages

**Actual Result:**  
- Trimmed successfully → login OK

**Status:** ✅ Passed  
**Tested on:** 2026-02-xx | Chrome 131 | Windows 11 | Desktop  
