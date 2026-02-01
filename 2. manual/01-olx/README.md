# 01 – OLX.pl

**Project Type:** Manual Testing – Functional & UI/UX  
**Tested Environment:**  
- Browser: Chrome 131 (latest)  
- OS: Windows 11  
- Device: Desktop (1920×1080)  
- Tested Date: January 2026  

**Scope of Testing:**  
- Authentication (Login)  
- Form validation (email & password)  
- Error handling & UX feedback  
- Basic usability features (button states, link visibility)

This project contains 18 test cases focused on the **login functionality** of OLX.pl.  
All test cases are written in a structured format and stored as individual Markdown files.

### Test Cases Overview

| ID     | Title                                              | Type          | Priority | Status  | Link to File                                                                 |
|--------|----------------------------------------------------|---------------|----------|---------|------------------------------------------------------------------------------|
| TC-001 | Login with valid credentials (Happy Path)          | Positive      | High     | Passed  | [TC-001_Login_Valid_credentials.md](test-cases/login/TC-001_Login_Valid_credentials.md) |
| TC-002 | Login after successful logout                      | Positive      | Medium   | Passed  | [TC-002_Login_After_successful_logout.md](test-cases/login/TC-002_Login_After_successful_logout.md) |
| TC-003 | Login using Enter key instead of button            | Positive      | Medium   | Passed  | [TC-003_Login_Using_Enter_key.md](test-cases/login/TC-003_Login_Using_Enter_key.md) |
| TC-004 | Successful login redirects to Moje OLX dashboard   | Positive      | High     | Passed  | [TC-004_Login_Successful_redirect_to_Moje_OLX.md](test-cases/login/TC-004_Login_Successful_redirect_to_Moje_OLX.md) |
| TC-005 | Invalid email format – no @ symbol                 | Negative      | High     | Passed  | [TC-005_Login_Invalid_email_no_at_symbol.md](test-cases/login/TC-005_Login_Invalid_email_no_at_symbol.md) |
| TC-006 | Invalid email format – no domain after @           | Negative      | High     | Passed  | [TC-006_Login_Invalid_email_no_domain.md](test-cases/login/TC-006_Login_Invalid_email_no_domain.md) |
| TC-007 | Non-existing email address                         | Negative      | Medium   | Passed  | [TC-007_Login_Non_existing_email.md](test-cases/login/TC-007_Login_Non_existing_email.md) |
| TC-008 | Empty email field                                  | Negative      | High     | Passed  | [TC-008_Login_Empty_email_field.md](test-cases/login/TC-008_Login_Empty_email_field.md) |
| TC-009 | Email with leading/trailing spaces (trimming)      | Positive      | Medium   | Passed  | [TC-009_Login_Email_with_leading_trailing_spaces.md](test-cases/login/TC-009_Login_Email_with_leading_trailing_spaces.md) |
| TC-010 | Invalid password                                   | Negative      | High     | Passed  | [TC-010_Login_Invalid_password.md](test-cases/login/TC-010_Login_Invalid_password.md) |
| TC-011 | Empty password field                               | Negative      | High     | Passed  | [TC-011_Login_Empty_password_field.md](test-cases/login/TC-011_Login_Empty_password_field.md) |
| TC-012 | Password with leading/trailing spaces (no trimming)| Negative      | Medium   | Failed  | [TC-012_Login_Password_with_leading_trailing_spaces.md](test-cases/login/TC-012_Login_Password_with_leading_trailing_spaces.md) |
| TC-013 | Password field masking (obfuscation)               | Positive      | High     | Passed  | [TC-013_Login_Password_field_masking.md](test-cases/login/TC-013_Login_Password_field_masking.md) |
| TC-014 | Error message for invalid credentials              | Negative      | High     | Passed  | [TC-014_Login_Error_message_for_invalid_credentials.md](test-cases/login/TC-014_Login_Error_message_for_invalid_credentials.md) |
| TC-015 | Error message disappears after correcting data     | Positive      | Medium   | Passed  | [TC-015_Login_Error_message_disappears_after_correction.md](test-cases/login/TC-015_Login_Error_message_disappears_after_correction.md) |
| TC-016 | Login button disabled when fields are empty        | Positive      | High     | Passed  | [TC-016_Login_button_disabled_when_fields_empty.md](test-cases/login/TC-016_Login_button_disabled_when_fields_empty.md) |
| TC-017 | Login button enabled after valid data entered      | Positive      | High     | Passed  | [TC-017_Login_button_enabled_after_valid_data.md](test-cases/login/TC-017_Login_button_enabled_after_valid_data.md) |
| TC-018 | "Forgot password" link visibility & functionality  | Positive      | High     | Passed  | [TC-018_Forgot_password_link_visibility_and_function.md](test-cases/login/TC-018_Forgot_password_link_visibility_and_function.md) |

### Related Defects

| ID      | Title                                              | Severity | Priority | Status | Link |
|---------|----------------------------------------------------|----------|----------|--------|------|
| BUG-001 | Missing spaces in subcategory labels (Nieruchomości) | Minor    | Low      | Open   | [BUG-001](../bug-reports/BUG-001_Missing_spaces_in_subcategory_labels_Nieruchomosci.md) |
| BUG-002 | Password field does not trim leading/trailing spaces | Minor    | Medium   | Open   | [BUG-002](../bug-reports/BUG-002_Password_field_does_not_trim_leading_trailing_spaces.md) |

### Learnings & Notes
- Strong client-side validation (empty fields, basic email format, button disabling)
- Good error messaging UX (specific, readable, disappears on correction)
- Weak point: No trimming of password whitespace → usability issue (linked bug)
- All tests reproducible on desktop Chrome – next: mobile/responsiveness checks

Feedback welcome!  
Feel free to open an issue or contact me.