# PARKEE QA Technical Test – Online Receipt

This repository contains test cases designed to validate the **Online Receipt** feature of the PARKEE parking system.

##Feature Overview
The **Online Receipt** allows users to scan a QR/barcode at the parking exit gate to view their parking transaction digitally, eliminating the need for paper receipts.

## Test Coverage

| Test Case ID | Scenario Description                              | Status |
|--------------|----------------------------------------------------|--------|
| TC001        | Scan valid barcode                                 | ✅ Pass |
| TC002        | Scan invalid/damaged barcode                       | ✅ Pass |
| TC003        | Access receipt manually via URL                    | ✅ Pass |
| TC004        | Access barcode after expiration (>24 hours)        | ✅ Pass |
| TC005        | Attempt access with no internet connection         | ✅ Pass |
| TC006        | Open receipt on unsupported/legacy browser         | ❌ Fail |
| TC007        | Camera permission denied while scanning            | ✅ Pass |
| TC008        | Validate receipt details (plate, time, fee)        | ✅ Pass |
| TC009        | Unauthorized access attempt to another’s receipt   | ✅ Pass |
| TC010        | Responsive display test on mobile devices          | ✅ Pass |

## Bugs Found

- **BUG001**: Online Receipt UI layout breaks on Internet Explorer 11.  
  _Suggestion_: Add warning for unsupported browsers or restrict access.

## 📁 Files Included

- `Test Case Parkee` – Detailed test scenarios, steps, expected & actual results.
- `README.md` – Overview and summary of the QA effort.
