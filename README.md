# SAP Capstone Project – Order-to-Cash (O2C) Complete Sales Cycle

---

## Student Details

| Field          | Details                          |
|----------------|----------------------------------|
| **Name**       | Ankit Raj                        |
| **Roll No.**   | 23051573                         |
| **Batch**      | B.Tech CSE                       |
| **Program**    | KIIT SAP Training Program        |
| **Module**     | SAP SD – Sales & Distribution    |
| **Topic**      | Order-to-Cash (O2C) – Complete Sales Cycle |
| **Submission** | April 21, 2026                   |

---

## Project Overview

This project demonstrates the complete **Order-to-Cash (O2C)** end-to-end business process
in **SAP SD (Sales & Distribution)** module for a fictitious company — **TechNova Pvt. Ltd.**

The O2C cycle is one of the most important business processes in any product-selling
enterprise. It covers every step from a customer inquiry to final payment receipt and clearing.

---

## Folder Structure

```
Ankit_Raj_SAP_O2C_Project/
│
├── README.md                          ← This file (Project Overview & Guide)
│
├── docs/
│   └── Ankit_Raj_SAP_O2C_Capstone_Project.pdf   ← Full Project Documentation (7 pages)
│
└── screenshots/
    ├── 01_VA01_Sales_Order_Creation.png           ← Step 3: Sales Order
    ├── 02_VL01N_Delivery_Goods_Issue.png          ← Step 4: Delivery & Goods Issue
    ├── 03_VF01_Billing_Invoice.png                ← Step 5: Invoice / Billing
    ├── 04_F28_Incoming_Payment_Clearing.png       ← Step 6: Payment Clearing
    └── 05_Document_Flow_O2C_Complete.png          ← Full Document Flow View
```

---

## O2C Process Steps Covered

| Step | Process                  | SAP Transaction | Description                                      |
|------|--------------------------|-----------------|--------------------------------------------------|
| 1    | Customer Inquiry         | VA11            | Customer expresses interest in products          |
| 2    | Quotation Creation       | VA21            | Formal price quote sent to customer              |
| 3    | Sales Order              | VA01            | Customer confirms order — core document          |
| 4    | Outbound Delivery        | VL01N           | Warehouse picks, packs, posts Goods Issue        |
| 5    | Billing / Invoice        | VF01            | Invoice raised, FI accounting entry auto-created |
| 6    | Payment Receipt          | F-28            | Customer payment posted, invoice cleared         |

---

## Key SAP Configuration Done

### Enterprise Structure
- **Company Code:** TN01 – TechNova Pvt. Ltd.
- **Sales Organization:** SO01
- **Distribution Channel:** DC01 – Direct Sales
- **Division:** DV01 – Electronics
- **Plant:** PL01 – Bengaluru Warehouse
- **Shipping Point:** SP01

### Master Data
- **Customer Master (XD01):** CUST001 – TechNova Customer
- **Material Master (MM01):** MAT-LAPTOP-01, MAT-MOUSE-01, MAT-BAG-01
- **Pricing Conditions (VK11):** PR00, K007, MWST (GST 18%)
- **Credit Limit (FD32):** INR 10,00,000

### Pricing Procedure
- **Procedure:** RVAA01
- **Conditions:** PR00 (Base Price) → K007 (Discount) → KF00 (Freight) → MWST (Tax)

---

## Screenshots Guide

| File Name                              | What It Shows                                      |
|----------------------------------------|----------------------------------------------------|
| `01_VA01_Sales_Order_Creation.png`     | VA01 screen with order items, ATP check passed, credit check passed |
| `02_VL01N_Delivery_Goods_Issue.png`    | Delivery document with picking status and GI posting confirmation |
| `03_VF01_Billing_Invoice.png`          | Invoice with net amount, GST, total, and FI accounting entry |
| `04_F28_Incoming_Payment_Clearing.png` | Payment posting with open item clearing — A/R reduced to zero |
| `05_Document_Flow_O2C_Complete.png`    | Full O2C document flow from Inquiry to Payment     |

---

## SAP Module Integration

```
SAP SD (Sales & Distribution)
        ↕
SAP FI  ← Billing document auto-generates accounting entries
SAP MM  ← Goods Issue reduces material stock
SAP WM  ← Transfer orders for warehouse picking
SAP CO  ← COGS posted to Controlling on GI
```

---

## Technologies Used

- **SAP ECC 6.0 / SAP S/4HANA**
- **SAP IMG (SPRO)** – Configuration
- **SAP SD, FI, MM, WM** modules
- **SAP GUI 7.70**

---

## Important Notes

- This is an **individual project** submitted as part of the KIIT SAP Capstone requirements.
- All screenshots depict the simulated SAP GUI environment for TechNova Pvt. Ltd.
- The PDF documentation follows the required format: A4, Arial font, justified, page numbers bottom-right.

---

## Declaration

I, **Ankit Raj** (Roll No: 23051573), hereby declare that this project is my own original
work prepared as part of the KIIT SAP Training Program Capstone submission.
The project has not been copied from any other source.

**Date:** April 21, 2026

---

*KIIT SAP Training Program | Capstone Project Submission | April 2026*
