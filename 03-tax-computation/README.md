# 04-Tax-Computation Portfolio Playbook

## 📊 Project Overview
This repository contains a professional, formula-driven tax computation engine built in Excel. The workbook successfully transitions a fictional UK entity (**BrightLeaf Interiors Ltd**) and an individual consultant from raw accounting profit into a fully adjusted, HMRC-aligned taxable profit baseline. 

This model serves as portfolio proof of skill for junior tax, accounting, and practice-readiness paths, replacing theoretical coursework with client-ready deliverables.

---

## 🛠️ Tools Used & Design Rules
* **Software:** Microsoft Excel / Google Sheets
* **Design Syntax:** Dynamic cross-referencing only (0% hardcoded intermediate calculations).
* **Tax Formatting:** Professional UK standard accounting format (`£#,##0;[Red](£#,##0);"-"`) featuring single-top underlines for subtotals and double-bottom lines for finalized tax liabilities.

---

## 🗂️ Workbook Architecture & Track Deliverables

The workbook is split into four highly organized, specialized calculation modules:

### 1. `01_Summary_README`
* **Purpose:** Acts as the executive roadmap and baseline control board.
* **Content:** Contextual profiles for both the individual consultant and the corporate entity, documenting baseline parameters and tax year metadata.

### 2. `02_Individual_Comp`
* **Purpose:** Converts a self-employed consultant's accounting net profit of **£62,000** into an adjusted tax result.
* **Adjustments:** Integrates automatic add-backs for disallowable items (depreciation, client entertainment blocks, personal cash drawings) and deducts linked capital allowances.
* **Tax Engine:** Uses dynamic `=MIN()` and `=MAX()` logic loops to accurately distribute income across the standard UK Personal Allowance (`£12,570`), Basic Rate Band (20%), and Higher Rate Band (40%).

### 3. `03_Corporate_Comp`
* **Purpose:** Performs corporate tax adjustment workflows starting from a Profit Before Tax (PBT) baseline of **£180,000**.
* **Adjustments:** Flags and resolves blocked expenses including capital legal fees, client hospitality, and depreciation adjustments.
* **Tax Engine:** Applies corporate slab metrics to derive the precise corporate cash tax liability.

### 4. `04_Working_Notes`
* **Purpose:** The foundational engine housing primary fixed-asset calculations.
* **Calculations:** Formulates capital allowance schedules, separating assets qualifying for the **100% Annual Investment Allowance (AIA)** from standard Main Pool items reducing at an **18% Writing-Down Allowance (WDA)** rate.
* **Integration:** Dynamically pushes outputs back to the tax computation schedules via cell linkages.

---

## 💡 Key Learning Outcomes & Professional Insights
* **Accrual vs. Tax Reconciliation:** Developed a thorough understanding of timing and permanent differences, specifically mastering the rule that accounting depreciation must **always** be added back and replaced by statutory capital allowances.
* **Spreadsheet Integrity:** Eliminated hardcoded values within calculation flows, ensuring the entire workbook dynamically rolls forward if base operational metrics change.
* **HMRC Compliance Awareness:** Gained practical exposure to identifying allowable vs. disallowable trading costs (e.g., distinguishing between allowable revenue repairs and disallowable capital improvements).

---

## 🔗 Portfolio Organization
To view the complete setup structure for this project within a larger portfolio ecosystem:
```text
finance-portfolio/
  📁 04-tax-computation/
    ├── README.md                 <-- (This Document)
    ├── 04-tax-computation.xlsx   <-- (Formula-Driven Excel Model)
```

---
*Created by akanksha kumari

