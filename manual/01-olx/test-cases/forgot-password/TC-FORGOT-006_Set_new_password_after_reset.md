# TC-FORGOT-006 – Set new password after clicking reset link

**Project:** OLX.pl  
**Module / Component:** Authentication → Forgot Password → New password setup  
**Type:** Positive  
**Priority:** High  
**Preconditions:**  
- A valid password reset link has been requested and received via email (as per TC-FORGOT-001)  
- The reset link has been clicked and the new password form is open  
- User has access to a strong, valid new password

**Test Data:**  
- New Password: NoweSilneHaslo2026!  
- Confirm Password: NoweSilneHaslo2026!

**Steps to Reproduce:**
1. Click the password reset link received in the email  
2. On the new password form, enter the new password in the "Wpisz nowe hasło" field  
3. Re-enter the same password in the confirmation field  
4. Click "Zapisz nowe hasło" button

**Expected Result:**
- Password is successfully updated  
- A success message is displayed (e.g. "Hasło zostało zmienione" or "Password changed successfully")  
- User is redirected to the login page or a confirmation page  
- Login with the new password is possible  
- Login with the old password is no longer possible

**Actual Result:** (during test)  
Success message: "Hasło zostało zmienione".  
User redirected to login page.  
Login with new password "NoweSilneHaslo2026!" succeeded.  
Login with previous password failed (correct behavior).

**Status:**  
✅ Passed

**Tested on:** 2026-02-01  
**Browser / OS / Device:** Chrome 131 | Windows 11 | Desktop 1920×1080  
**Environment:** Production

**Attachments / Evidence:**  
- ![TC-FORGOT-006 – success message after setting new password](evidence/TC-FORGOT-006_success-message-new-password.png)   
- ![TC-FORGOT-006 – login failure with old password](evidence/TC-FORGOT-006_login-failure-old-password.png)  

