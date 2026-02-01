# TC-002 – Login after successful logout

**Project:** OLX.pl  
**Module:** Authentication → Login form  
**Type:** Positive  
**Priority:** Medium  
**Preconditions:**  
- User is already logged in with valid credentials

**Test Data:** Same as TC-001

**Steps to Reproduce:**
1. Perform successful login (follow TC-001)
2. Hover over "Twoje konto" in the top-right corner
3. Click "Wyloguj się"
4. After logout, click "Twoje konto" again
5. Select "Zaloguj się"
6. Enter the same valid email and password
7. Click "Zaloguj się"

**Expected Result:**
- User is logged out successfully (no longer sees personalized content)
- Subsequent login with the same credentials succeeds
- Redirects back to "Moje OLX"
- No errors

**Actual Result:** [Same as expected – success]

**Status:** ✅ Passed