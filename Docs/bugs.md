# 🐞 Bugs Found

---

## 🟠 BUG001 - Email Verification Template Breaks Layout With Long Verification URL

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

<img width="1874" height="956" alt="msedge_2026-06-01_00-28-08" src="https://github.com/user-attachments/assets/6b1a4632-f974-45a0-89cd-00ac220b5395" />


---

## 🟡 BUG002 - Chat Widget Overlaps reCAPTCHA Security Information

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
<img width="1564" height="956" alt="msedge_2026-05-31_02-27-13" src="https://github.com/user-attachments/assets/8d90f893-b779-4ba3-be36-4fe5f119ac7f" />
<img width="1564" height="956" alt="msedge_2026-05-31_02-27-50" src="https://github.com/user-attachments/assets/8f8f22ec-614d-40e6-be2f-ad18da03e873" />



---

## 🟠 BUG003 - Password Setup Flow Fails After User Remains Idle

**Severity:** Medium

**Priority:** High

**Description:**

When a newly created user remains idle on the password setup screen for approximately 30 minutes to 1 hour, the password creation flow fails and the user cannot complete the onboarding process.

Although this scenario may not happen frequently, it can occur if a user starts creating the account and gets interrupted before setting the password.

**Steps to Reproduce:**

1. Create a new Metrobi account
2. Access the password setup screen
3. Remain idle on the page for approximately 30 minutes to 1 hour
4. Try to create the password
5. Submit the form

**Expected Result:**

- User should be able to complete the password creation successfully
- If the session expires, the system should display a clear and user-friendly message
- User should be redirected to reauthenticate or request a new valid password setup link

**Actual Result:**

- Password creation fails
- User cannot proceed with the onboarding flow
- System returns the following error:

{
  "error": {
    "code": 400,
    "message": "CREDENTIAL_TOO_OLD_LOGIN_AGAIN",
    "errors": [
      {
        "message": "CREDENTIAL_TOO_OLD_LOGIN_AGAIN",
        "domain": "global",
        "reason": "invalid"
      }
    ]
  }
}

**Technical Observation:**   
The authentication credential used during password setup appears to expire after a period of inactivity.

The application does not handle the expired credential state gracefully and exposes a raw authentication error instead of guiding the user to recover the flow.

The only identified workaround is using the "Forgot Password" flow

**Evidence:**  
[[Click the image to see the video]<img width="1834" height="936" alt="image" src="https://github.com/user-attachments/assets/0def7365-b95a-4b79-bfba-7f735b084600" />](https://github.com/user-attachments/assets/bafbac25-c348-4130-93cc-1f588cc57d67)


---

## 🟠 BUG004 - Invalid Email Error Message Persists After Successful Account Creation

**Severity:** Medium

**Priority:** Medium

**Description:**

When creating a new account, if the user first enters an invalid email address, the system correctly displays an email validation error.

However, after the user replaces the invalid email with a valid one and successfully creates the account, the previous validation error message is still displayed on the account creation confirmation page.

**Steps to Reproduce:**

1. Access the account creation page
2. Fill in the form using an invalid email address
3. Submit the form
4. Observe the email validation error message
5. Replace the invalid email with a valid email address
6. Submit the form again
7. Observe the account creation confirmation page

**Expected Result:**

- The invalid email error message should disappear after the user corrects the email
- The confirmation page should only display information related to the successful account creation
- No previous validation errors should be shown after a successful submission

**Actual Result:**

- The account is successfully created
- The confirmation page is displayed
- The previous invalid email error message remains visible on the confirmation page

**Technical Observation:**

The validation error state appears to persist after successful form submission.  
The application may not be clearing the previous error message before rendering the account creation confirmation state.

**Evidence:**  

<img width="500" height="701" alt="msedge_2026-05-31_23-26-24" src="https://github.com/user-attachments/assets/cc9a208e-0a7d-428f-b368-6ec9769be082" />
<img width="1874" height="995" alt="msedge_2026-05-30_15-08-05" src="https://github.com/user-attachments/assets/6f00f9d2-3437-42fa-b402-0c4d56fb3435" />



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

