# TC-007 – Login attempt with non-existing email address

**Project:** OLX.pl  
**Module:** Authentication → Login form  
**Type:** Negative – Server-side validation  
**Priority:** Medium  
**Preconditions:** Valid password known

**Test Data:**  
- Email: nieistniejący@example.com  
- Password: PoprawneHaslo123!

**Steps to Reproduce:**
1. Navigate to login page
2. Enter non-existing email
3. Enter valid password
4. Click "Zaloguj się"

**Expected Result:**
- Error message indicating invalid credentials, e.g. "E-mail jest nieprawidłowy" or generic "Nieprawidłowe dane logowania"
- User stays on login form, no access granted

**Actual Result:**  
- Message: "Coś poszło nie tak..."  
- Login blocked (correct security behavior – avoids username enumeration)

**Status:** ✅ Passed 