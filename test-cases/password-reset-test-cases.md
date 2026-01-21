# Password Reset Test Cases

This document contains manual test cases for the password reset functionality.

---

## Test Case 1: Request password reset with registered email

**Precondition:** User has an existing account

**Steps:**
1. Navigate to the Login page
2. Click on "Forgot password"
3. Enter a registered email address
4. Click "Submit"

**Expected Result:**
- Password reset confirmation message is displayed
- Reset email is sent to the user

---

## Test Case 2: Request password reset with unregistered email

**Steps:**
1. Navigate to the Login page
2. Click on "Forgot password"
3. Enter an unregistered email address
4. Click "Submit"

**Expected Result:**
- Generic message is shown (e.g., "If an account exists...")
- No sensitive information is revealed

---

## Test Case 3: Reset password using valid reset link

**Precondition:** User has received a valid reset email

**Steps:**
1. Open the password reset email
2. Click on the reset link
3. Enter a valid new password
4. Confirm the new password
5. Click "Save"

**Expected Result:**
- Password is successfully updated
- User is redirected to the login page

---

## Test Case 4: Reset password with expired or invalid link

**Steps:**
1. Open an expired or invalid reset link
2. Attempt to reset the password

**Expected Result:**
- Error message is displayed
- User is prompted to request a new reset link

---

## Test Case 5: Reset password with weak password

**Steps:**
1. Open a valid reset link
2. Enter a weak password (e.g., 12345)
3. Confirm the password
4. Click "Save"

**Expected Result:**
- Password strength validation error is shown
- Password is not updated
