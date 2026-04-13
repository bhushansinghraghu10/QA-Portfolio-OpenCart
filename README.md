# 🧪 QA Portfolio — Manual Testing of OpenCart E-Commerce Platform

![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![Test Cases](https://img.shields.io/badge/Test%20Cases-40-blue)
![Pass Rate](https://img.shields.io/badge/Pass%20Rate-80%25-green)
![Bugs Found](https://img.shields.io/badge/Bugs%20Found-8-red)
![Type](https://img.shields.io/badge/Type-Manual%20Testing-orange)

---

## 📌 About This Project

End-to-end **manual QA testing** of [OpenCart](https://demo.opencart.com) — a live, open-source e-commerce web application used by thousands of businesses worldwide.

This project simulates a complete, real-world **Software Testing Life Cycle (STLC)** — from test planning through execution, defect reporting, and a final test summary report — using industry-standard documentation formats.

> **Tester:** Bhushan Singh | **Date:** April 2026 | **Environment:** Chrome (Latest) on Windows 11

---

## 🎯 Objectives

- Validate functional quality across 5 core application modules
- Design structured test cases using proven test design techniques
- Identify, classify, and document real defects with reproducible steps
- Produce professional QA deliverables that reflect industry standards
- Demonstrate end-to-end QA workflow independently

---

## 🔬 Scope of Testing

| Module | Test Cases | Testing Types Applied |
|--------|-----------|----------------------|
| User Registration & Login | 8 | Positive, Negative, Boundary, Security |
| Product Search & Filters | 7 | Positive, Negative, Boundary, Security |
| Shopping Cart & Checkout | 10 | Positive, Negative, Boundary, Equivalence |
| Wishlist & Comparison | 8 | Positive, Negative, State-based |
| Contact Us / Form Validation | 7 | Positive, Negative, Boundary |
| **TOTAL** | **40** | |

---

## 📊 Execution Results

| Metric | Value |
|--------|-------|
| Total Test Cases Written | 40 |
| Total Executed | 40 |
| ✅ Passed | 32 |
| ❌ Failed | 8 |
| 🚫 Blocked | 0 |
| **Pass Rate** | **80%** |

---

## 🐛 Defects Found

| Bug ID | Module | Bug Title | Severity | Priority | Status |
|--------|--------|-----------|----------|----------|--------|
| BUG_001 | Registration | Duplicate email shows unclear error message | Medium | High | Open |
| BUG_002 | Registration | Password < 4 characters accepted | **High** | High | Open |
| BUG_003 | Login | No account lockout after 10 failed attempts | **High** | High | Open |
| BUG_004 | Search | Blank search returns all products silently | Medium | High | Open |
| BUG_005 | Search | Price filter min > max shows no validation error | Medium | Medium | Open |
| BUG_006 | Cart | Cart accepts quantity = 0 without error | **High** | High | Open |
| BUG_007 | Cart | Cart accepts negative quantity values | **High** | High | Open |
| BUG_008 | Contact Us | Form submits with spaces-only message | Medium | Medium | Open |

### Defect Severity Breakdown
```
High Severity   ████████ 4 defects  (50%)
Medium Severity ████████ 4 defects  (50%)
Low Severity             0 defects
```

---

## 🛠 Test Design Techniques Used

| Technique | Applied In |
|-----------|-----------|
| **Boundary Value Analysis** | Password length, quantity fields, price range |
| **Equivalence Partitioning** | Valid/invalid email, search terms, form inputs |
| **Negative Testing** | Wrong credentials, invalid data, blank submissions |
| **Exploratory Testing** | Wishlist behaviour, checkout edge cases |
| **Basic Security Testing** | SQL injection in search/login, input sanitization |

---

## 📁 Repository Structure

```
QA-Portfolio-OpenCart/
│
├── README.md
│
├── Test-Plan/
│   └── OpenCart_Test_Plan.pdf          ← Scope, objectives, approach, entry/exit criteria
│
├── Test-Cases/
│   └── OpenCart_TestCases_BugReport.xlsx   ← 40 test cases + bug report + summary dashboard
│
├── Bug-Reports/
│   └── OpenCart_TestCases_BugReport.xlsx   ← JIRA-format bug log (same file, Bug Report sheet)
│
├── Test-Summary-Report/
│   └── OpenCart_Test_Summary_Report.pdf    ← Executive summary, metrics, verdict
│
└── Screenshots/
    └── Bug_001.png through Bug_008.png     ← Screenshot evidence for each defect
```

---

## 🔧 Tools Used

| Tool | Purpose |
|------|---------|
| Microsoft Excel | Test case management, bug tracking (JIRA-format) |
| Google Chrome | Test execution browser |
| Windows Snipping Tool | Bug screenshot capture |
| GitHub | Version control and portfolio hosting |
| reportlab / openpyxl | Document generation (PDF, Excel) |

---

## 📋 Deliverables

| Artifact | Description | Format |
|----------|-------------|--------|
| Test Plan | Scope, approach, environment, entry/exit criteria | PDF |
| Test Case Suite | 40 executed test cases with Pass/Fail status | Excel |
| Bug Report Log | 8 defects in JIRA-format with steps + screenshots | Excel |
| Test Summary Report | Metrics, module results, verdict, recommendations | PDF |
| Screenshots | Visual evidence for all 8 defects | PNG |

---

## 🏁 Conclusion & Recommendation

> ❌ **NOT RECOMMENDED FOR RELEASE** without resolving High-severity defects.

4 High-severity defects were identified — including cart quantity validation failures (zero and negative values accepted) and a login brute-force vulnerability (no account lockout). A targeted bug-fix cycle followed by **regression testing** of the Cart and Login modules is recommended before production deployment.

---

## 👤 About the Tester

**Bhushan Singh** — Detail-oriented B.Tech graduate with hands-on experience in QA workflows, structured test documentation, and data validation.

- 📧 bhushansinghraghu10@gmail.com
- 💼 [LinkedIn](https://www.linkedin.com/in/)
- 📍 Delhi NCR, India

---

*This project was conducted independently as part of a QA portfolio. All testing was performed on the publicly available OpenCart demo environment.*
