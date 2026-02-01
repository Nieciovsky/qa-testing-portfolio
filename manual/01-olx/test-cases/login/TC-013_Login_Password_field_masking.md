# TC-013 – Password field masks entered characters

**Project:** OLX.pl  
**Module:** Authentication → Login form → Security / UX  
**Type:** Positive – Security feature  
**Priority:** High  
**Preconditions:** Login form open

**Test Data:** Any password (e.g. PoprawneHaslo123!)

**Steps to Reproduce:**
1. Navigate to login page
2. Click into "Hasło" field
3. Start typing characters
4. Observe the field content

**Expected Result:**
- Entered characters are masked (displayed as dots ••••• or asterisks *****)
- No plain text visible on screen

**Actual Result:**  
- Characters masked as dots (•••••)
- Correct password obfuscation

**Status:** ✅ Passed  
