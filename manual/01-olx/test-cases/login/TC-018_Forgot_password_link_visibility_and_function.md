# TC-018 – "Forgot password" link is visible and functional

**Project:** OLX.pl  
**Module:** Authentication → Login form → Recovery features  
**Type:** Positive – Accessibility / Usability  
**Priority:** High  
**Preconditions:**  
- Login form is displayed

**Test Data:** None required (visibility & navigation check)

**Steps to Reproduce:**
1. Navigate to https://www.olx.pl
2. Click "Twoje konto" in the top-right corner
3. Select "Zaloguj się"
4. Locate the "Nie pamiętam hasła" link on the login form
5. Click the link
6. Observe the navigation outcome

**Expected Result:**
- Link is clearly visible (proper contrast, size, position)
- Link is clickable
- Clicking redirects to the password reset / recovery page/form
- No errors during navigation

**Actual Result:**  
- Link is visible and well-positioned  
- Clicking successfully navigates to the password reset flow

**Status:** ✅ Passed  
