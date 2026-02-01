# TC-FORGOT-007 – Set new password with leading/trailing spaces during reset

**Project:** OLX.pl  
**Module / Component:** Authentication → Forgot Password → Password input sanitization  
**Type:** Negative / Usability  
**Priority:** Medium  
**Preconditions:**  
- Valid password reset link has been clicked  
- New password setup form is open  
- User has access to the reset flow

**Test Data:**  
- New Password: `"  NoweHaslo2026!  "` (with leading and trailing spaces)  


**Steps to Reproduce:**
1. Click the password reset link from the email  
2. In the "Wpisz nowe hasło" field, enter the password with leading and trailing spaces  
3. In the confirmation field, enter the exact same value (with spaces)  


**Expected Result:**
- Best practice: system automatically trims leading/trailing spaces  
- Password is saved without the extra spaces  
- Success message appears  
- Login is possible with the trimmed password ("NoweHaslo2026!")  
- Login fails if using version with spaces

**Actual Result:**  
Error symbol displayed next to "Password" field.  
No trimming occurred – spaces were treated as part of the password.  
"Set password" button is NOT active.
Password change failed.  
This matches the non-trimming behavior observed in login (see BUG-002).

**Status:**  
❌ Failed

**Tested on:** 2026-02-01  
**Browser / OS / Device:** Chrome 131 | Windows 11 | Desktop 1920×1080  
**Environment:** Production

**Attachments / Evidence:**  
- ![TC-FORGOT-007 – error after entering password with spaces](evidence/TC-FORGOT-007_error-spaces-in-new-password.png)  
- ![TC-FORGOT-007 – input field showing spaces](evidence/TC-FORGOT-007_error-spaces-in-new-password.png)  

