# TC-FORGOT-005 – Reset link expiration

**Project:** OLX.pl  
**Module / Component:** Authentication → Forgot Password → Link validity  
**Type:** Negative / Boundary  
**Priority:** Medium  
**Preconditions:**  
- A valid password reset link has been requested and received via email  
- The link has not been used yet  
- Access to the email inbox is available

**Test Data:**  
- Email: testqa001@example.com  
- Reset link: the link received in the email from a previous reset request

**Steps to Reproduce:**
1. Request a password reset using a valid email (as in TC-FORGOT-001)  
2. Receive and save/copy the reset link from the email  
3. Wait a sufficient time for the link to expire (based on OLX policy; typically 24–48 hours)  
4. After the waiting period, open the saved reset link in the browser

**Expected Result:**
- An error message is displayed indicating the link has expired (e.g. "Link wygasł", "Proszę wygenerować nowy link", or "This link is no longer valid")  
- The user is unable to set a new password using the expired link  
- No password change is applied  
- Option to request a new reset link is available

**Actual Result:** (during test)  


**Status:**  
⌛ InProgress

**Tested on:** 2026-02-01 to 2026-02-02  
**Browser / OS / Device:** Chrome 131 | Windows 11 | Desktop 1920×1080  
**Environment:** Production

**Attachments / Evidence:**  


