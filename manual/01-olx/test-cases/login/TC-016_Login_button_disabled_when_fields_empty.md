# TC-016 – Login button disabled when email and password fields are empty

**Project:** OLX.pl  
**Module:** Authentication → Login form → Form controls / UX  
**Type:** Positive – Client-side validation / Usability  
**Priority:** High  
**Preconditions:**  
- Login page is open  
- No data entered yet

**Test Data:**  
- Email: (empty)  
- Password: (empty)

**Steps to Reproduce:**
1. Navigate to https://www.olx.pl
2. Click "Twoje konto" in the top-right corner
3. Select "Zaloguj się"
4. Observe the "Zaloguj się" button state with:
   - both fields empty
   - email empty, password filled
   - email filled, password empty

**Expected Result:**
- "Zaloguj się" button is disabled (grayed out, not clickable) as long as either or both fields are empty
- Prevents submission of incomplete form

**Actual Result:**  
- Button remains disabled in all three cases until both fields are filled  
- Correct client-side behavior

**Status:** ✅ Passed  