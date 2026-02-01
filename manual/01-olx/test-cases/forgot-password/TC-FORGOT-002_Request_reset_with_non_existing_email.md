# TC-FORGOT-002 – Request password reset with non-existing email

**Project:** OLX.pl  
**Module / Component:** Authentication → Forgot Password  
**Type:** Negative  
**Priority:** Medium  
**Preconditions:**  
- User is logged out  
- Forgot password form is open  
- No access to the email inbox is required for this test (only frontend/server response checked)

**Test Data:**  
- Email: nieistniejacy1234567890abcdef@example.com (non-registered, obviously fake address)

**Steps to Reproduce:**
1. Go to https://www.olx.pl  
2. Click "Twoje konto" in the top-right corner  
3. Select "Zaloguj się"  
4. Click "Nie pamiętam hasła" link/button  
5. Enter the non-existing email address in the email field  
6. Click "Wyślij link" / "Resetuj hasło"

**Expected Result:**
- An error message is displayed (specific like "Taki adres e-mail nie jest zarejestrowany" or generic "Coś poszło nie tak...")  
- No password reset email is sent  
- User remains on the forgot password form  
- No unexpected redirects or page crashes

**Actual Result:** (during test)  
Generic error message displayed: "Coś poszło nie tak. Spróbuj ponownie później."  
No email received in any inbox (checked spam/junk too).  
User stayed on the form. No reset link generated.

**Status:**  
✅ Passed

**Tested on:** 2026-02-01  
**Browser / OS / Device:** Chrome 131 | Windows 11 | Desktop 1920×1080 

**Attachments / Evidence:**  
- ![TC-FORGOT-002 – error message for non-existing email](evidence/TC-FORGOT-002_error-non-existing-email.png)  
