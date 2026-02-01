# TC-004 – Successful login redirects to correct dashboard

**Project:** OLX.pl  
**Module:** Authentication → Post-login redirect  
**Type:** Positive  
**Priority:** High  
**Preconditions:** Valid credentials

**Test Data:** Same as TC-001

**Steps to Reproduce:**
1. Perform successful login (as in TC-001)

**Expected Result:**
- Immediate redirect to "Moje OLX" dashboard or main account page
- URL changes appropriately (e.g. contains /konto/ or similar)
- No intermediate error pages or loops

**Actual Result:** [Same as expected – success]

**Status:** ✅ Passed