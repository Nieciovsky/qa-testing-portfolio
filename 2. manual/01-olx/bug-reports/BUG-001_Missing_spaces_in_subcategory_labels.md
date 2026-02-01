# BUG-001 – Missing spaces in subcategory labels (Nieruchomości menu)

**Project:** OLX.pl  
**Module/Component:** Main navigation → Category "Nieruchomości" dropdown  
**Type:** UI / Typographical  
**Reported:** 2026-01-12  
**Environment:**
- Browser: Chrome 131 (latest)
- OS: Windows 11
- Resolution: 1920×1080
- Device: Desktop
- User state: Both logged-in and logged-out (reproducible)

**Steps to Reproduce:**
1. Open https://www.olx.pl
2. Click on the main category „Nieruchomości”
3. Observe the subcategory labels in the bottom row of the dropdown menu

**Actual Result:**
Several subcategory labels are missing spaces between words, e.g.:
- „Ogródw Dom i Ogród” insted of „Ogród w Dom i Ogród”
- „Budowa i Remontw Usługi” insted of „Budowa i Remont w Usługi”

**Expected Result:**
All subcategory labels are correctly formatted with proper spaces, e.g.:
- „Ogród w Dom i Ogród”
- „Budowa i Remont w Usługi”

**Severity:** Minor / Cosmetic 
**Priority:** Low

**Attachments / Evidence:**
![BUG-001 - Missing spaces in subcategory labels](https://github.com/user-attachments/assets/3ede5451-6f72-4196-ab32-23d586fd444c)
