# TC-FORGOT-001 – Request password reset with valid registered email

**Project:** OLX.pl  
**Module / Component:** Authentication → Forgot Password  
**Type:** Positive  
**Priority:** High  
**Preconditions:**  
- User has a registered and confirmed email account  
- User is logged out  
- Browser opened in normal mode  
- Access to the email inbox is available

**Test Data:**  
- Email: testqa001@example.com (existing, registered email)

**Steps to Reproduce:**
1. Go to https://www.olx.pl  
2. Click "Twoje konto" in the top-right corner  
3. Select "Zaloguj się"  
4. Click "Nie pamiętam hasła" link/button  
5. Enter the registered email in the email field  
6. Click "Wyślij link" / "Resetuj hasło"

**Expected Result:**
- Success message appears on the page (e.g. "Link został wysłany na Twój adres e-mail")  
- An email with a password reset link is received within a reasonable time (usually < 1 minute)  
- The email contains a valid-looking reset link  
- No error messages are shown on the page  
- User stays on the login / info page

**Actual Result:** (during test)  
Success message displayed: "Link został wysłany". Email arrived within ~10 seconds with valid reset link. No errors.

**Status:**  
✅ Passed

**Tested on:** 2026-02-01  
**Browser / OS / Device:** Chrome 131 | Windows 11 | Desktop 1920×1080 

**Attachments / Evidence:**  
- ![TC-FORGOT-001 – success message after request](../evidence/TC-FORGOT-001_success-message-after-request.png)  
- ![TC-FORGOT-001 – reset email received](../evidence/TC-FORGOT-001_reset-email-received.png)  

**Notes / Observations:**
- Test ends here (email received and link visible).  
- Setting new password is checked separately in TC-FORGOT-006  