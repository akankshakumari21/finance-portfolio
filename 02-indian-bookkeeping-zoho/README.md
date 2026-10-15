# Project 1: Full-Cycle Indian Corporate Bookkeeping & Statutory Tax Architecture
### **Platform Engine:** Zoho Books Cloud Sandbox  
### **Base Currency:** INR (₹)  
### **Fictional Entity Case Study:** Vedic Decor Private Limited (Home Furnishings Sector)

---

## 📌 Project Executive Summary
This project demonstrates the execution of a complete, end-to-end bookkeeping and statutory tax cycle for a simulated Indian retail corporation. The workflow involves transitioning unorganized raw operational receipts, supplier invoices, and customer billing into a fully balanced, audit-ready financial statement pack. 

The system configuration strictly enforces compliance under the **Central Goods and Services Tax (CGST) Act**, rules governing **Input Tax Credit (ITC)** reclaims, **Section 194C TDS withholding codes**, and institutional banking controls.

---

## 🛠️ System Configuration & Tax Matrix
* **Accounting Framework:** Double-Entry Accrual Bookkeeping
* **Core Sales Tax Ambit:** Local GST @ 18% (9% CGST + 9% SGST)
* **Inventory Control HSN:** `940360` (Wooden Corporate & Domestic Furniture)
* **Withholding Interface:** Income Tax Section 194C (Contractor Payment Deductions)
* **Reconciliation Target Account:** HDFC Bank Current Account

---

## 📊 Core Financial Deliverables & Reconciled Metrics

### 1. General Ledger Balance (Trial Balance)
* **Total Net Debits:** ₹2,95,000.00 | **Total Net Credits:** ₹2,95,000.00  
* *Audit Check:* The system records a perfect zero-variance matching matrix across all active asset, liability, expense, and revenue categories.

### 2. Profit & Loss Statement (Operating Performance)
* **Gross Operating Income (Sales):** ₹1,00,000.00
* **Total Operating Expenses:** ₹61,090.00
* **Net Operating Profit:** ₹38,910.00  
* *Expense Breakdown:* Transportation (₹50,000), Motor Fuel (₹5,000), Corporate Entertaining (₹3,500), Office Supplies (₹2,000), Bank Fees (₹590).

### 3. Balance Sheet Snapshot (Financial Position)
* **Total Balanced Assets:** ₹2,33,910.00 | **Total Liabilities & Equities:** ₹2,33,910.00
* **Liquid Position:** Reconciled Cash & Bank Equiv. sitting at ₹47,550.00 (HDFC Bank: ₹43,410 | Petty Cash: ₹4,140).

### 4. Statutory Compliance Netting (GST & TDS Ledgers)
* **Output GST Liability:** ₹18,000.00 (₹9,000 Output CGST + ₹9,000 Output SGST)
* **Eligible Input Tax Credit (ITC Asset):** ₹9,360.00 (₹4,680 Input CGST + ₹4,680 Input SGST)
* **Withholding Tax Obligation:** ₹1,000.00 (TDS Payable under Section 194C)

---

## 🔍 Local Compliance Adjustments Handled Successfully
1. **GST Destination Logic:** Mapped split intra-state tax routines on gross billing values, ensuring duties auto-populated into the respective state and central tax ledger pools.
2. **Blocked Credit Exclusions (Section 17(5)):** Identified and manually isolated ₹3,500 under *Meals and Entertainment*. While the vendor invoice carried a tax profile, the credit was marked as *Ineligible ITC* per Indian tax statutes, forcing the cost to be completely absorbed by the business.
3. **Granular TDS Withholding:** Applied a 2% withholding deduction on a ₹50,000 freight invoice from *Apex Logistics Ltd*. The transaction accurately reduced cash outflow, established a ₹1,000 liability to the Income Tax Department, and properly captured the remaining base cost.
4. **Bank Reconciliation (BRS):** Manually matched physical bank statements against ledger lines. Tracked and processed a hidden ₹590 auto-debit line (₹500 net bank charge + 18% financial services GST) to completely align the software balance with the statement closing figure.

---

## 📁 Repository Directory Structure
All verified financial statement outputs have been exported as immutable data assets and stored using the following folder conventions:
```text
📁 finance-portfolio/
  📁 01-indian-bookkeeping-zoho/
    📄 README.md                  <-- (This Project Landing Page)
    📁 reports/
      📄 01-gst-summary-gstr3b.json <-- (Raw Schema Return Code)
      📄 02-trial-balance.pdf        <-- (Debit/Credit Proof)
      📄 03-profit-and-loss.pdf      <-- (Performance Statement)
      📄 04-balance-sheet.pdf        <-- (Financial Position Snapshot)
```

