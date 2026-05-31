# 🐞 Bugs Found

---

## ⚠️ BUG001 - Email Verification Template Breaks Layout With Long Verification URL

**Severity:**  Medium     
**Priority:**  Medium 

**Description:**   
After creating a new account, the email verification template does not properly handle long verification URLs. The fallback verification link exceeds the content container boundaries, causing layout issues and visual inconsistencies within the email body.

**Steps to Reproduce:**
1. Create a new account
2. Receive the verification email
3. Open the email
4. Scroll to the fallback verification link section

**Expected Result:**  
- Verification link should wrap correctly inside the email container
- Email content should remain properly aligned
- Background container should maintain visual integrity

**Actual Result:**  
- Verification URL overflows outside the intended content area
- Text alignment becomes inconsistent
- Background section appears visually broken or incomplete

**Technical Observation:**   
The email template appears not to handle large URL strings correctly. Missing word-wrap or overflow handling may be causing the layout to break in some email clients.

**Evidence:**  
image

---

## ⚠️ BUG002 - Chat Widget Overlaps reCAPTCHA Security Information

**Severity:**  Low   
**Priority:**  Low 

**Description:**   
On the account creation confirmation page, the chatbot widget overlaps the reCAPTCHA security notice displayed in the bottom-right corner of the screen.

**Steps to Reproduce:**
1. Create a new account
2. Reach the account creation confirmation page
3. Wait for the chatbot widget to load
4. Observe the bottom-right corner

**Expected Result:**  
- reCAPTCHA information should remain fully visible
- Chat widget should not cover compliance or security-related information

**Actual Result:**  
- Chat widget partially overlaps the reCAPTCHA security notice
- Part of the information becomes hidden from the user

**Technical Observation:**   
The widget appears to use a fixed position without considering the reserved space required by Google's reCAPTCHA disclosure.

**Evidence:**  
image

---

## ⚠️ BUG003 - Asd

**Severity:**  Low   
**Priority:**  Low 

**Description:**   
asd

**Steps to Reproduce:**
1. asd  
2. asd
3. asd
4. asd

**Expected Result:**   
- asd
- asd

**Actual Result:**   
- asd
- asd

**Technical Observation:**   
asd

**Evidence:**  
image

---

## ⚠️ BUG004 - Asd

**Severity:**  Low   
**Priority:**  Low 

**Description:**   
asd

**Steps to Reproduce:**
1. asd  
2. asd
3. asd
4. asd

**Expected Result:**   
- asd
- asd

**Actual Result:**   
- asd
- asd

**Technical Observation:**   
asd

**Evidence:**  
image

---

## ⚠️ BUG005 - Asd

**Severity:**  Low   
**Priority:**  Low 

**Description:**   
asd

**Steps to Reproduce:**
1. asd  
2. asd
3. asd
4. asd

**Expected Result:**   
- asd
- asd

**Actual Result:**   
- asd
- asd

**Technical Observation:**   
asd

**Evidence:**  
image

---

## ⚠️ BUG006 - Asd

**Severity:**  Low   
**Priority:**  Low 

**Description:**   
asd

**Steps to Reproduce:**
1. asd  
2. asd
3. asd
4. asd

**Expected Result:**   
- asd
- asd

**Actual Result:**   
- asd
- asd

**Technical Observation:**   
asd

**Evidence:**  
image


**Evidence:**  
image

