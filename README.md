# Metrobi Exploratory Testing Challenge

## Objective

Perform exploratory testing on the Metrobi shipper dashboard and document findings.

## Test Approach

The application was tested using an exploratory testing approach focused on validating the main user workflows, navigation, data validation, account management, and delivery management features.  
The goal was not only to identify defects but also to evaluate the overall user experience, consistency of validations, and behavior of the application under different scenarios.

## Areas Tested

During the exploratory session, the following sections were reviewed:

### Deliveries

* My Deliveries
* Daily View
* Incoming Deliveries
* Delivery Settings
* Create Delivery flow

### Drivers

* Metrobi Network
* Self Managed Drivers
* Driver Feedback

### Customers

* Customer listing
* Customer details
* Invoices section

### Chats

* Chat interface
* AI Agent conversation

### Settings

* Company Details
* Users management
* Profile settings
* API Keys management
* Billing

### Account Creation & Onboarding

* User registration
* Password creation flow
* Session handling
* Form validations

## Results

### Bugs Found

| ID     | Title                                                                                   | Severity |
| ------ | --------------------------------------------------------------------------------------- | -------- |
| BUG001 | Email Verification Template Breaks Layout With Long Verification URL                    | Medium   |
| BUG002 | Chat Widget Overlaps reCAPTCHA Security Information                                     | Low      |
| BUG003 | Password Setup Flow Fails After User Remains Idle                                       | Medium   |
| BUG004 | Invalid Email Error Message Persists After Successful Account Creation                  | Medium   |
| BUG005 | Invalid and Duplicate Email Can Be Added as a New User                                  | High     |

## Additional Observations

### OBS001 - API Keys Are Permanently Visible

Generated API keys remain fully visible in the interface after creation and after page refresh.  
While this behavior does not prevent functionality, many systems mask API keys after creation and only display them once to reduce accidental credential exposure.  
This was recorded as an observation rather than a defect because the expected behavior was not explicitly defined.

## Environment

* Browser: Microsoft Edge, Google Chrome
* Operating System: Windows 11, Mobile Emulation (IOS, Android)
* Tab Navigation (Accessibility)

## Documentation

Detailed bug reports and supporting evidence can be found in:

* `Docs/bugs.md`
