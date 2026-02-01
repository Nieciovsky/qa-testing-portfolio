# TC-017 – Login button becomes enabled after entering valid data

**Project:** OLX.pl  
**Module:** Authentication → Login form → Form controls / UX  
**Type:** Positive – Form interactivity  
**Priority:** High  
**Preconditions:**  
- Login page open  
- Fields initially empty → button disabled

**Test Data:**  
- Email: test@example.com  
- Password: PoprawneHaslo123!

**Steps to Reproduce:**
1. Navigate to login page (steps 1–3 from TC-016)
2. Enter valid email in "E-mail" field
3. Enter valid password in "Hasło" field
4. Observe the "Zaloguj się" button state

**Expected Result:**
- Button changes from disabled to enabled (becomes clickable, color/normal state changes)
- User can submit the form and log in successfully

**Actual Result:**  
- Button becomes active and clickable after both fields are filled  
- Successful login possible

**Status:** ✅ Passed  