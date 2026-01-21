# Signup Test Cases

This document contains manual test cases for the Signup / Registration functionality.

---

## Test Case 1: Signup with valid inputs

**Precondition:** User is not logged in  
**Steps:**
1. Navigate to the Signup page
2. Enter a valid email
3. Enter a strong password (meets requirements)
4. Confirm the same password (if required)
5. Click the Sign up / Create account button

**Expected Result:**
- Account is created successfully
- User is redirected to dashboard or verification page
- A success message is shown

---

## Test Case 2: Signup with already registered email

**Precondition:** Email is already registered  
**Steps:**
1. Navigate to the Signup page
2. Enter an existing email address
3. Enter a valid password
4. Click Sign up

**Expected Result:**
- Signup is blocked
- Error message indicates email is already in use
- User is prompted to log in or reset password

---

## Test Case 3: Signup with invalid email format

**Steps:**
1. Navigate to the Signup page
2. Enter an invalid email (e.g., selma@)
3. Enter a valid password
4. Click Sign up

**Expected Result:**
- Validation error is shown for email
- Account is not created

---

## Test Case 4: Signup with weak password

**Steps:**
1. Navigate to the Signup page
2. Enter a valid email
3. Enter a weak password (e.g., 12345)
4. Click Sign up

**Expected Result:**
- Validation error is shown for password requirements
- Account is not created

---

## Test Case 5: Signup with mismatched password confirmation

**Steps:**
1. Navigate to the Signup page
2. Enter a valid email
3. Enter a password
4. Enter a different password in Confirm Password
5. Click Sign up

**Expected Result:**
- Error message indicates passwords do not match
- Account is not created
