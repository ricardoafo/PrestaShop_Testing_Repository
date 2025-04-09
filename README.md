# Manual Testing Documentation

This directory contains all the manual testing artifacts for the **PrestaShop Testing Portfolio**. It is organized to clearly separate traditional test documentation from behavior-driven development (BDD) formats.

## Structure

```
Manual_Testing/
├── Test_Plan.md
├── Common_Test_Cases/
│   ├── HomePage_TestCases.md
│   ├── Cart_TestCases.md
├── Gherkin_Test_Cases/
│   ├── homepage.feature
│   ├── search.feature
├── Bug_Reports/
│   ├── Bug_Report_Template.md
│   ├── Bug_001.md
```

---

## Test_Plan.md
This file outlines the **overall test strategy**, scope, objectives, types of testing, and entry/exit criteria based on ISTQB standards.

---

## Common_Test_Cases/
Contains **classic/manual test cases** written in table format (ID, steps, expected result, priority, etc.).  
These are useful for documentation, manual test execution, or uploading to test case management tools like TestRail, Xray, or Zephyr.

---

## Gherkin_Test_Cases/
Contains test scenarios written in **Gherkin language (`.feature` files)** using the Given-When-Then format.  
These are compatible with Cucumber and useful for BDD workflows, test automation planning, or collaborative documentation.

---

## Bug_Reports/
Includes structured **bug report templates** and actual reported bugs during manual testing.  
Each bug file includes:
- Title
- Steps to reproduce
- Expected vs. actual result
- Severity and priority
- Screenshots or references if needed

---
