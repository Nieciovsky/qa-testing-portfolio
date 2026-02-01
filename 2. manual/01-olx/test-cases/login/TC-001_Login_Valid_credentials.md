# TC-001 – Login with valid email and password (Happy Path)

**Project:** OLX.pl  
**Module:** Authentication → Login form  
**Type:** Positive  
**Priority:** High  
**Preconditions:**  
- User has a valid, active account on OLX.pl  
- Browser is opened in normal mode (not incognito)

**Test Data:**  
- Email: test@example.com  
- Password: PoprawneHaslo123!

**Steps to Reproduce:**
1. Navigate to https://www.olx.pl
2. Click "Twoje konto" in the top-right corner
3. Select "Zaloguj się"
4. Enter the email address in the "E-mail" field
5. Enter the password in the "Hasło" field
6. Click the "Zaloguj się" button

**Expected Result:**
- User is successfully logged in
- Page redirects to "Moje OLX" dashboard / user panel
- No error messages are displayed
- User's name / avatar appears in the top-right corner

**Actual Result:** 
[Same as expected – success]

**Status:** ✅ Passed  
**Tested on:** 2026-02-xx | Chrome 131 | Windows 11 | Desktop