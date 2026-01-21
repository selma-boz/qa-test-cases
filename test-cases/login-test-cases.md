# Login Test Cases

This document contains manual test cases for the Login functionality.

---

## Test Case 1: Login with valid credentials
**Precondition:** User has a registered account  
**Steps:**
1. Navigate to the Login page
2. Enter a valid email
3. Enter a valid password
4. Click the Login button

**Expected Result:**  
User is logged in successfully and redirected to the dashboard.

---

## Test Case 2: Login with invalid password
**Precondition:** User has a registered account  
**Steps:**
1. Navigate to the Login page
2. Enter a valid email
3. Enter an invalid password
4. Click the Login button

**Expected Result:**  
An error message is displayed indicating incorrect credentials.

---

## Test Case 3: Login with empty fields
**Steps:**
1. Navigate to the Login page
2. Leave email and password fields empty
3. Click the Login button

**Expected Result:**  
Validation messages are shown for required fields.
