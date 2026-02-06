# 📌 01 – OLX.pl

**🔸 Project Type:** Manual Testing – Functional & UI/UX  <br><br>
**🔸Tested Environment:**  
- Browser: Chrome 131 (latest)  
- OS: Windows 11  
- Device: Desktop (1920×1080)  
- Tested Date: January–February 2026  

**🔸 Scope of Testing:**  
- Authentication (Login & Forgot Password)  
- Form validation (email & password)  
- Error handling & UX feedback  
- Basic usability features (button states, link visibility, cancellation)

<br>

<p align="center"> 🔹 This project contains 26 test cases with bug reports focused on the <b>authentication functionality</b> of OLX.pl (Login + Forgot Password). 🔹<br> 
🔹 All test cases are written in a structured format and stored as individual Markdown files. 🔹</p>
<br><br>

# 📚 Scope of Contents:
1. [Test Cases Overview – Login](#LoginLogin)
2. [Test Cases Overview – Forgot Password](#ForgotPasswordPassword)
3. [Releted Defects](#RelatedDefects)
4. [Learnings & Notes](#Learnings)

<br>


<h3 id="LoginLogin">📋 Test Cases Overview – Login </h3>

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

<h3 id="ForgotPasswordPassword">📋 Test Cases Overview – Forgot Password </h3>

| ID          | Title                                              | Type          | Priority | Status  | Link to File                                                                 |
|-------------|----------------------------------------------------|---------------|----------|---------|------------------------------------------------------------------------------|
| TC-FORGOT-001 | Request password reset with valid registered email | Positive      | High     | Passed  | [TC-FORGOT-001_Request_reset_with_valid_email.md](test-cases/forgot-password/TC-FORGOT-001_Request_reset_with_valid_email.md) |
| TC-FORGOT-002 | Request password reset with non-existing email     | Negative      | Medium   | Passed  | [TC-FORGOT-002_Request_reset_with_non_existing_email.md](test-cases/forgot-password/TC-FORGOT-002_Request_reset_with_non_existing_email.md) |
| TC-FORGOT-003 | Request password reset with invalid email format   | Negative      | High     | Passed  | [TC-FORGOT-003_Request_reset_with_invalid_email_format.md](test-cases/forgot-password/TC-FORGOT-003_Request_reset_with_invalid_email_format.md) |
| TC-FORGOT-004 | Multiple password reset requests (rate limiting)   | Negative / Security | Medium   | Passed  | [TC-FORGOT-004_Multiple_reset_requests_rate_limiting.md](test-cases/forgot-password/TC-FORGOT-004_Multiple_reset_requests_rate_limiting.md) |
| TC-FORGOT-005 | Reset link expiration                              | Negative / Boundary | Medium   | Passed  | [TC-FORGOT-005_Reset_link_expiration.md](test-cases/forgot-password/TC-FORGOT-005_Reset_link_expiration.md) |
| TC-FORGOT-006 | Set new password after clicking reset link         | Positive      | High     | Passed  | [TC-FORGOT-006_Set_new_password_after_reset.md](test-cases/forgot-password/TC-FORGOT-006_Set_new_password_after_reset.md) |
| TC-FORGOT-007 | Set new password with leading/trailing spaces      | Negative / Usability | Medium   | Failed  | [TC-FORGOT-007_New_password_with_leading_trailing_spaces.md](test-cases/forgot-password/TC-FORGOT-007_New_password_with_leading_trailing_spaces.md) |
| TC-FORGOT-008 | Cancel or back button during reset flow            | Positive / Usability | Medium   | Passed  | [TC-FORGOT-008_Cancel_or_back_during_reset_flow.md](test-cases/forgot-password/TC-FORGOT-008_Cancel_or_back_during_reset_flow.md) |

<h3 id="RelatedDefects">📛  Related Defects </h3>

| ID      | Title                                              | Severity | Priority | Status | Link |
|---------|----------------------------------------------------|----------|----------|--------|------|
| BUG-001 | Missing spaces in subcategory labels (Nieruchomości) | Minor    | Low      | Open   | [BUG-001](../01-olx/bug-reports/BUG-001_Missing_spaces_in_subcategory_labels.md) |
| BUG-002 | Password field does not trim leading/trailing spaces (login) | Minor    | Medium   | Open   | [BUG-002](../01-olx/bug-reports/BUG-002_Password_field_does_not_trim_leading_trailing_spaces.md) |
| BUG-003 | No trimming of new password during reset flow      | Minor    | Medium   | Open   | [BUG-003](../01-olx/bug-reports/BUG-003_No_trimming_new_password_reset.md) |

<br>

<h3 id="Learnings"> 🧠 Learnings & Notes </h3>

- Strong client-side validation across login and forgot password forms (empty fields, email format, button disabling) <br>
- Good error messaging UX (specific where possible, disappears on correction, generic for security) <br>
- Weak point: No trimming of password whitespace – occurs both in login (BUG-002) and reset flow (BUG-003) → usability issue <br>
- Rate limiting on reset requests is strong (60-minute block after ~7 attempts) – excellent protection against abuse <br>
- All tests reproducible on desktop Chrome – next steps: mobile/responsiveness checks and additional modules (search, ad posting) <br>
- Authentication coverage now includes: login (18 TC), forgot password (8 TC), total 26 TC + 3 bugs <br>


Feedback welcome!  
Feel free to open an issue or contact me.
