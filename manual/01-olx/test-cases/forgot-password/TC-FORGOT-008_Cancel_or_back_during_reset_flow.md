# TC-FORGOT-008 – Cancel or back button during password reset flow

**Project:** OLX.pl  
**Module / Component:** Authentication → Forgot Password → Navigation / Usability  
**Type:** Positive / Usability  
**Priority:** Medium  
**Preconditions:**  
- Forgot password form or new password setup form is open  
- User is in the middle of the reset password flow (e.g. after entering email or after clicking reset link)

**Test Data:**  
- None required (navigation / cancellation test)

**Steps to Reproduce:**
1. Go to https://www.olx.pl  
2. Click "Twoje konto" in the top-right corner  
3. Select "Zaloguj się"  
4. Click "Nie pamiętam hasła" link/button  
5. Enter any email address (valid or invalid)  
6. Before clicking "Zmień", click "Anuluj" / browser back button  


**Expected Result:**
- User is returned to the login page or main page  
- No password reset email is sent (if cancelled before submit)  
- No changes are applied to the account  
- No error messages or unexpected behavior occur  
- The reset flow is cleanly interrupted

**Actual Result:**
Clicking "Anuluj" / browser back button link successfully returned user to the login form.  
No email was sent (checked inbox).  
No errors or page crashes. Flow interrupted correctly without side effects.

**Status:**  
✅ Passed

**Tested on:** 2026-02-01  
**Browser / OS / Device:** Chrome 131 | Windows 11 | Desktop 1920×1080  
**Environment:** Production