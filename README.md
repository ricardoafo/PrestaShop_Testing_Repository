# 🛍️ PrestaShop QA Project

This repository provides a complete QA setup for the [PrestaShop Demo Store](https://demo.prestashop.com/#/en/front), covering both **manual** and **automated testing** with best practices in structure, reporting, and CI/CD.

---

## 📁 Project Structure

```plaintext
prestashop-qa/
├── manual-tests/                 # Manual test cases and documentation
│   ├── TestCases.csv             # Traditional test cases (CSV format)
│   ├── features/                 # Gherkin scenarios for manual tests
│   └── manual-test-plan.md      # ISTQB-style test plan
├── automation/                  # Playwright + Cucumber automated tests
│   ├── features/                # Gherkin BDD features for automation
│   ├── steps/                   # Step definitions in TypeScript
│   ├── pages/                   # Page Object Model classes
│   ├── hooks/                   # Cucumber hooks (Before/After)
│   ├── support/utils/           # Reusable utils and selectors
│   └── reports/                 # HTML & trace reports
├── config/                      # Cucumber, Playwright, and environment config
├── docker/                      # Docker container setup for automation
├── .github/workflows/           # GitHub Actions workflows for CI
├── package.json                 # NPM scripts and dependencies
└── README.md                    # This file
```

---

## 🧪 Manual Testing

- Structured using CSV files and Gherkin syntax.
- Located in `manual-tests/`
- Aligned with ISTQB best practices.
- Covers functional, usability, and exploratory testing.

---

## 🤖 Automation Framework

Built with:

- [Playwright](https://playwright.dev/) for browser automation.
- [TypeScript](https://www.typescriptlang.org/) for reliability and maintainability.
- [Cucumber.js](https://github.com/cucumber/cucumber-js) for BDD (Given/When/Then).
- [Docker](https://www.docker.com/) for consistent local and CI environments.
- [GitHub Actions](https://github.com/features/actions) for CI execution.

### Features

- ✅ Cross-browser testing (Chromium, Firefox, WebKit)
- ✅ Mobile viewport simulation
- ✅ Page Object Model structure
- ✅ Cucumber HTML reporting
- ✅ Visual regression support (screenshots)
- ✅ Runs locally or in Docker

---

## 🐳 Running in Docker

```bash
docker build -t prestashop-tests -f docker/Dockerfile .
docker run --rm prestashop-tests
```

Or use Docker Compose:

```bash
docker-compose up --build
```

---

## 🚀 Run Locally

Install dependencies:

```bash
npm install
npx playwright install
```

Run tests:

```bash
npm run test
```

---

## 📊 Reports

Reports are generated in `/automation/reports/` and include:

- HTML test result reports
- Screenshots on failure
- Playwright trace viewer (optional)

---

## 📌 GitHub Actions

CI pipeline runs all tests across supported browsers and uploads test artifacts.

---

## 👤 Author

**Ricardo Afonso**  
📅 April 2025  
📫 r.afonsomontero@gmail.com