📄 Program Name
ZSR_TEST_VIKAS
An ABAP Report that generates a Smart Form output of Purchase Order (PO) details from SAP standard tables.
-----------------------------------------------------------------------------------------------------------------------------------------
🧾 Overview
This SAP ABAP project is designed to generate a formatted Purchase Order report using Smart Forms. The report fetches PO headers and their line items (EKKO and EKPO tables) 
based on a user-specified posting date range and passes the data to the Smart Form: ZPURCHASING_DOCUMENT_HEADER.

----------------------------------------------------------------------------------------------------------------------------------------------------------

# SAP ABAP Smart Form Project - Purchase Order Report

## 📄 Program Name
`ZSR_TEST_VIKAS`

## 📚 Description
This report fetches purchase order data (`EKKO`, `EKPO`) based on a date range and outputs the data using a Smart Form (`ZPURCHASING_DOCUMENT_HEADER`).

## 🧩 Components
- **Tables Used**: `EKKO`, `EKPO`
- **Custom Structure**: `ZSR_TEST_VIKAS` (should be defined in Data Dictionary)
- **Smart Form**: `ZPURCHASING_DOCUMENT_HEADER`

## 🚀 How It Works
1. User provides date range through select-options.
2. The report fetches PO headers and corresponding PO line items with non-zero quantity.
3. Data is collected into internal tables and passed to Smart Form.
4. Smart Form prints the details.

## 📦 How to Use
1. Import the program `zsr_test_vikas.abap` in your SAP system.
2. Ensure Smart Form `ZPURCHASING_DOCUMENT_HEADER` is available in the system.
3. Execute the program with appropriate date range.

## 📌 Notes
- Material number is replaced by `<Service PO>` in case it is blank.
- Field `menge` is excluded from output, but can be added back if needed.

---
