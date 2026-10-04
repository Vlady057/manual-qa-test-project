
# Test Plan

## 1. Introduction

This test plan describes the testing approach for the SauceDemo web application.

The purpose of testing is to verify the functionality of the main user flows and identify defects that may affect the user experience.

## 2. Test Objectives

The main objectives are:

* Verify user authentication.
* Verify product catalog functionality.
* Verify product sorting.
* Verify product details.
* Verify shopping cart functionality.
* Verify checkout functionality.
* Verify order completion.
* Identify and document defects.
* Ensure that the main user flow works as expected.

## 3. Scope

### 3.1 In Scope

The following functionality will be tested:

* Login
* Logout
* Product catalog
* Product sorting
* Product details
* Add product to cart
* Remove product from cart
* Shopping cart
* Checkout form
* Checkout validation
* Order overview
* Order completion

### 3.2 Out of Scope

The following areas are not included:

* Performance testing
* Load testing
* Security testing
* API testing
* Database testing
* Mobile application testing
* Accessibility testing
* Cross-browser compatibility testing

## 4. Test Types

The following testing types will be used:

### Functional Testing

Verification that application functionality works according to expected behavior.

### Smoke Testing

Verification of the main application functionality before detailed testing.

### Regression Testing

Verification that previously working functionality continues to work after changes.

### Negative Testing

Verification of application behavior when invalid or unexpected data is provided.

### Exploratory Testing

Unscripted testing used to identify unexpected behavior and potential defects.

### UI Testing

Verification of visible interface elements, navigation, labels, buttons, and basic layout.

## 5. Test Environment

| Parameter        | Value                      |
| ---------------- | -------------------------- |
| Application      | SauceDemo                  |
| URL              | https://www.saucedemo.com/ |
| Operating System | Windows                    |
| Browser          | Google Chrome              |
| Testing Type     | Manual                     |
| Environment      | Web                        |

## 6. Test Data

### Standard User

```text
Username: standard_user
Password: secret_sauce
```

### Checkout Data

```text
First Name: Volodymyr
Last Name: QA
Zip/Postal Code: 10001
```

## 7. Entry Criteria

Testing can start when:

* The application is accessible.
* The test environment is available.
* Valid test credentials are available.
* Main application functionality is accessible.

## 8. Exit Criteria

Testing can be completed when:

* Planned test cases have been executed.
* Critical functionality has been verified.
* Identified defects have been documented.
* Test results have been recorded.
* Test summary has been prepared.

## 9. Risks

Potential risks include:

* Application changes during testing.
* Unexpected application behavior.
* Browser-specific issues.
* Test environment availability.
* Previously unknown application defects.

## 10. Deliverables

The following documents will be created as part of testing:

* Test Plan
* Test Scenarios
* Test Cases
* Checklist
* Bug Reports
* Test Summary Report

## 11. Test Execution Approach

Testing will follow the main user workflow:

```text
Login
  ↓
Products
  ↓
Product Details
  ↓
Cart
  ↓
Checkout
  ↓
Order Overview
  ↓
Order Completion
```

Test cases will be executed manually and the actual results will be compared with the expected results.

Identified defects will be documented using structured bug reports containing:

* Bug ID
* Title
* Preconditions
* Steps to Reproduce
* Expected Result
* Actual Result
* Severity
* Priority
* Environment
* Status
