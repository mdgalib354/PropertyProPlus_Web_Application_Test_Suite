## PropertyProPlus QA Test Management
This repository contains the comprehensive QA documentation and test case management for the PropertyProPlus (SaaS) application. The documentation focuses on verifying core functionalities, third-party integrations (Valex, Scribe, Xero), and valuation workflows.

---------------

## Project Overview

Project Name: PropertyProPlus
Application: PropertyProPlus (SaaS)
Test Objective: Verify core functionalities, integrations, and workflows work correctly.
Test Type: Manual Functional Testing
Environment: Web Application (Staging/Test Environment)

---------------

## Documentation Structure

The testing suite is organized into two primary components:

Test Plan: Outlines the scope, objectives, and environment details for the QA cycle.

Test Result (Excel/CSV): 
• A detailed repository of 70+ test cases covering:
• Valex & AnyDesk integration.
• Scribe Sketch integration and webhook calling.
• Xero/MYOB invoicing workflows.
• Mortgage vs. Non-Mortgage valuation forms.
• User role management and permission logic.

Regression/Bug Reports (Word Document): Detailed steps for reproducing specific defects found during the copy-valuation and data-persistence workflows.

---------------

## Key Test Areas
1. Valuation Lifecycle
   
Creation: Testing the "Order a Valuation" flow through Valex and internal web forms.
Workflow Actions: Verifying status transitions (e.g., New VLX Job -> Unassigned -> Accepted -> Payment Received).
Duplication: Ensuring data consistency and field clearing (SWOT analysis, Title Details, Appointment Dates) when copying existing valuations.

2. Integrations
   
Scribe Sketch: Testing the connection between the web portal and Scribe, including area calculations and drawing persistence.
Financials: Validating Xero invoice generation and automated status updates via webhooks upon payment.
Valex: End-to-end testing of job creation from external Funder platforms.

3. Role & Permissions
   
Testing transitions between Valuer, Client, and Admin roles.
Verification of UI elements based on Scribe subscription status.

---------------

## How to Use the Test Suite

Execution: Refer to the TC_ID in the PropertyProPlus_QA_Full_Test_Management.xlsx file.
Reproduction: For failed cases (marked as Fail in the status column), use the detailed Test Steps and Actual Result columns to reproduce the issues.
Data Requirements: Ensure the environment has active Scribe and Valex test credentials as specified in the Test_Data fields.

---------------

Prepared and Executed by: Asadullah Al-Galib
