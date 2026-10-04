# Manual QA Test Project

Manual testing project for the SauceDemo web application.

The project demonstrates a complete manual QA workflow including test planning, test scenarios, test cases, checklists, bug reporting, and test summary.

## Application Under Test

**Application:** SauceDemo
**Type:** E-commerce web application
**Testing Type:** Manual Testing
**Environment:** Web Browser
**URL:** https://www.saucedemo.com/

## Project Objectives

The main objectives of this project are:

* Verify the main functionality of the web application.
* Check user authentication.
* Test product catalog functionality.
* Verify product sorting.
* Test shopping cart functionality.
* Test checkout functionality.
* Verify order completion.
* Identify and document defects.
* Demonstrate practical Manual QA skills.

## Scope

### In Scope

* Login
* Product catalog
* Product sorting
* Product details
* Shopping cart
* Checkout form
* Checkout overview
* Order completion
* Basic UI validation
* Functional testing
* Negative testing

### Out of Scope

* Performance testing
* Load testing
* Security testing
* API testing
* Database testing
* Mobile application testing
* Cross-browser compatibility testing

## Test Documentation

| Document                                          | Description                                      |
| ------------------------------------------------- | ------------------------------------------------ |
| [Test Plan](test-plan/test-plan.md)                | Test objectives, scope, environment and strategy |
| [Test Scenarios](test-scenarios/test-scenarios.md) | High-level testing scenarios                     |
| [Test Cases](test-cases/test-cases.md)             | Detailed test cases with expected results        |
| [Checklist](checklists/checklist.md)               | Functional testing checklist                     |
| [Bug Reports](bug-reports/bug-reports.md)          | Documented defects                               |
| [Test Summary](test-summary/test-summary.md)       | Final testing results                            |

## Testing Areas

### Authentication

* Valid login
* Invalid login
* Empty credentials
* Login validation

### Products

* Product list
* Product information
* Product sorting
* Product details

### Shopping Cart

* Add product
* Remove product
* Multiple products
* Cart contents
* Cart navigation

### Checkout

* Checkout form
* Required fields
* Invalid input
* Order overview
* Order completion

## Test Types

The following testing techniques are used:

* Functional Testing
* Smoke Testing
* Regression Testing
* Negative Testing
* UI Testing
* Exploratory Testing
* Boundary Value Analysis
* Equivalence Partitioning

## Test Environment

| Parameter        | Value         |
| ---------------- | ------------- |
| Application      | SauceDemo     |
| Platform         | Windows       |
| Browser          | Google Chrome |
| Testing Type     | Manual        |
| Test Environment | Web           |

## Project Structure

```text
manual-qa-test-project/
│
├── README.md
│
├── test-plan/
│   └── test-plan.md
│
├── test-cases/
│   └── test-cases.md
│
├── test-scenarios/
│   └── test-scenarios.md
│
├── checklists/
│   └── checklist.md
│
├── bug-reports/
│   └── bug-reports.md
│
├── test-summary/
│   └── test-summary.md
│
└── docs/
    └── screenshots/
```
