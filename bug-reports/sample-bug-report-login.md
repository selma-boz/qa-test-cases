# Bug Report: Login fails with correct credentials after password reset

## Summary
**Title:** Login fails with correct credentials after password reset  
**Module/Area:** Authentication / Login  
**Environment:** macOS, Chrome (latest)  
**Build/Version:** N/A  
**Reporter:** Selma Boz  
**Date:** 2026-01-21  

---

## Description
After resetting the password successfully, the user cannot log in using the new password. The login page shows a generic error message.

---

## Steps to Reproduce
1. Go to the Login page.
2. Click **Forgot password**.
3. Enter a valid email and submit.
4. Open the reset link from the email.
5. Set a new password and confirm.
6. Return to Login and enter the same email + the new password.
7. Click **Log in**.

---

## Actual Result
Login fails and an error message appears (e.g., “Something went wrong” / “Invalid credentials”), even though the new password was set successfully.

---

## Expected Result
User should be able to log in successfully with the new password immediately after resetting it.

---

## Frequency / Reproducibility
- [x] Always (100%)

---

## Severity
- [x] Major

## Priority
- [x] P1 (High)

---

## Impact
Users who reset their password are blocked from accessing their account, increasing support requests and reducing user trust.

---

## Attachments / Evidence
- Screenshot(s): (add later)
- Video: (add later)
- Console logs: (add later)
- Network logs: (add later)

---

## Notes
Possible caching/session issue after password reset. Try clearing cookies or logging out all sessions after reset.
