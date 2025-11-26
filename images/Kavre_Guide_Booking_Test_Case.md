# QA Artifact: Kavre Guide Tourism Platform - Test Strategy & Case

## 1. Context and Strategy (Derived from SAD/SE Reports)

This document demonstrates the planning required for the Quality Assurance (QA) phase of the 'Kavre Guide' platform.

### **Testing Approach**
* **Methodology:** Primarily **Manual Black-Box Testing** to verify all functional requirements against the original design specifications (DFDs, Use Cases).
* **Focus Areas:** High-priority modules include the Guide Booking System, User Authentication, and critical database interactions.
* **Goal:** Ensure a robust, secure, and user-centric experience for both Tourists and Guides.

---

## 2. Sample Detailed Functional Test Case

This test case verifies the most critical business function: booking a guide.

| Field | Description |
| :--- | :--- |
| **Test Case ID** | **TC-BOOK-001** |
| **Test Objective** | To verify a Tourist can successfully search and complete a booking request for an available guide. |
| **Test Condition** | Tourist is logged in; Guide is marked as 'Available' on the desired date. |

### Test Steps (Execution Flow)

| Step # | Action | Expected Result (Success Criteria) |
| :--- | :--- | :--- |
| **1** | Navigate to the "Search Guides" page and filter by location and date. | The system displays available guides matching the criteria quickly (Performance check). |
| **2** | Select a guide and fill out the Booking Form with valid details. | The form accepts all required input (Name, Date, Party Size) and validates email format. |
| **3** | Submit the booking request. | **Critical:** A success message is displayed on the screen AND a booking request confirmation email is sent to the Tourist. |
| **4** | (System Check) A notification is sent to the Guide. | The Guide's Dashboard updates to show a **New Pending** booking request. |

---
