# TC-015 – Error message disappears after correcting invalid credentials

**Project:** OLX.pl  
**Module:** Authentication → Login form → Error handling / UX  
**Type:** Positive – Error state recovery  
**Priority:** Medium  
**Preconditions:**  
- Previous failed login attempt with error message visible (e.g. from TC-010 or TC-014)

**Test Data (corrected):**  
- Email: test@example.com  
- Password: PoprawneHaslo123! (valid)

**Steps to Reproduce:**
1. Perform a failed login attempt to trigger error message (invalid credentials)
2. Observe the displayed error message
3. Clear or correct the invalid field(s) – enter valid email and password
4. Click "Zaloguj się" again
5. Observe the error message behavior and login outcome

**Expected Result:**
- Error message disappears immediately or after submit
- Successful login occurs
- Redirect to "Moje OLX" dashboard
- No residual error messages remain visible

**Actual Result:** 
- Error message disappears after entering correct credentials  
- Successful login and redirect to "Moje OLX"  
- Clean form state after success

**Status:** ✅ Passed  
