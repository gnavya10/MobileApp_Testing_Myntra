#  Myntra Mobile Application Testing Documentation

##  Introduction

This document outlines the end-to-end test strategy for the **Myntra Mobile Application**. The purpose is to validate all core functionalities, ensure usability, and deliver a seamless shopping experience across Android and iOS platforms.

---

##  Test Approach

- **Manual Testing:** Used for UI/UX, exploratory, and usability tests.
- **Cross-Platform Testing:** Ensures consistency across Android and iOS devices.
- **Functional Testing:** To validate individual functionalities like login, search, cart, etc.
- **Non-Functional Testing:** Includes performance, usability, network handling, and offline behavior.

---

## Roles and Responsibilities

| Role                | Responsibility                                                  |
|---------------------|------------------------------------------------------------------|
| QA Lead             | Define test strategy, coordinate testing effort, report progress|
| Manual Testers      | Execute test cases, report bugs                                 |
| Developers          | Fix defects and collaborate with QA                             |
| Product Owner       | Requirement gathering, approval of test outcomes                |

---

##  Entry Criteria

- Functional requirements are finalized and shared.
- Test environment is ready.
- Test data is prepared.
- Build is deployed and stable.

##  Exit Criteria

- All critical and high-priority test cases have been executed.
- No high-severity bugs remain open.
- All test cases have passed or acceptable workarounds are in place.
- Test summary report is submitted and approved.

---

##  Mind Map of Functionalities

![Myntra Mobile App Mindmap](Link - )

---

##  Test Scenarios Summary

| Module                | Test Scenarios Covered |
|------------------------|------------------------|
| Login & Signup         | 14 Test Cases          |
| Search Functionality   | 10 Test Cases          |
| Cart & Wishlist        | 10 Test Cases          |
| Checkout & Payment     | 5 Test Cases           |
| Orders & Invoices      | 3 Test Cases           |
| Notifications & Offline Handling | 4 Test Cases   |
| Logout & Re-login      | 2 Test Cases           |
| App Data & State Resume| 2 Test Cases           |

Total: **50 Test Cases**

---

##  Sample Bug Report

**Title:** App does not resume from last state, the session is refreshed.

- **Priority:** High
- **Severity:** Medium to High
- **Environment:** ios 15, Myntra 4.2503.20
- 
- **Steps to Reproduce:**
  1. Open the app and navigate to product details
  2.Scroll through the products and switch the application
  3. Reopen after a few minutes
- **Expected Result:** App should resume from the same state
- **Actual Result:** App restarts and redirects to home page or else the section is refreshed.

---

##  Sample Test Case (Login Module)

| Test Case ID | Test Scenario               | Test Case Description                     | Pre-Requisites        |
|--------------|-----------------------------|-------------------------------------------|------------------------|
| TC_001       | Verify Login Functionality   | Signup/Login button is clickable          | Install Myntra Application and Login |
| TC_002       | Verify Login Functionality   | Able to log in with valid credentials     | Install Myntra Application and Login |
| TC_004       | Verify Phone OTP Login       | Verify signup with phone + OTP            | Install Myntra Application and Login |
| TC_008       | Verify Sign up with Empty    | Sign up with no inputs                    | Install Myntra Application and Login |
| ...          | ...                          | ...                                       | ...                    |

---

##  Tools Suggested

- **Manual Testing:** JIRA, TestRail, Excel
- **Bug Tracking:** JIRA, Bugzilla
- **Documentation:** Confluence, Markdown

---



