# TC-FORGOT-004 – Multiple password reset requests in short time (rate limiting)

**Project:** OLX.pl  
**Module / Component:** Authentication → Forgot Password → Rate limiting / Security  
**Type:** Negative / Security  
**Priority:** Medium  
**Preconditions:**  
- User is logged out  
- Forgot password form is open  
- Valid registered email is available for testing  
- Access to the email inbox is available (to check if emails are sent)

**Test Data:**  
- Email: testqa001@example.com (existing, registered email)

**Steps to Reproduce:**
1. Go to https://www.olx.pl  
2. Click "Twoje konto" in the top-right corner  
3. Select "Zaloguj się"  
4. Click "Nie pamiętam hasła" link/button  
5. Enter the valid registered email  
6. Click "Wyślij link" → observe success message and check email inbox  
7. Immediately repeat steps 5–6 (enter same email and click "Wyślij link") 8–10 times within 1–2 minutes

**Expected Result:**
- First few requests succeed (email sent each time)  
- After several attempts (typically 5–10), a rate limiting protection activates:  
  - Error message appears (e.g. "Zbyt wiele prób. Spróbuj ponownie za kilka minut" or CAPTCHA challenge)  
  - Further requests are temporarily blocked (no more emails sent)  
  - Block lasts for a reasonable time (e.g. 5–15 minutes)

**Actual Result:**   
First 4 requests succeeded (emails arrived each time).  
On the 5th attempt: message "Przez najbliższą godzinę nie możemy wysłać Ci więcej kodów. Nie możesz znaleźć e-maila od nas? Sprawdź w folderze spam. Jeśli go tam nie ma, spróbuj później lub skontaktuj się z nami." appeared.  
No further emails sent for the next 60 minutes. Rate limiting behavior confirmed.

**Status:**  
✅ Passed

**Tested on:** 2026-02-01  
**Browser / OS / Device:** Chrome 131 | Windows 11 | Desktop 1920×1080  


**Attachments / Evidence:**  
- ![TC-FORGOT-004 – rate limit message after multiple requests](evidence/TC-FORGOT-004_rate-limit-message.png)  
- ![TC-FORGOT-004 – multiple emails received before block](evidence/TC-FORGOT-004_multiple-emails-before-block.png)  

**Notes**
Rate limiting triggered after 5 consecutive requests within ~2 minutes.
Block duration: 60 minutes (no further reset emails could be requested).
After 60 minutes, the reset request worked normally again.