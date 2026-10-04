
# Test Summary Report

## 1. Test Execution Summary

Testing was performed for the main functionality of the SauceDemo web application.

The following areas were covered:

* Login
* Products
* Product Details
* Product Sorting
* Shopping Cart
* Checkout
* Checkout Overview
* Order Completion
* Navigation
* Logout

## 2. Test Environment

| Parameter        | Value                      |
| ---------------- | -------------------------- |
| Application      | SauceDemo                  |
| URL              | https://www.saucedemo.com/ |
| Operating System | Windows                    |
| Browser          | Google Chrome              |
| Testing Type     | Manual                     |
| Environment      | Web                        |

## 3. Test Results

A total of **28 test cases** were documented and evaluated.

| Result          |        Count |
| --------------- | -----------: |
| Passed          |           22 |
| Failed          |            6 |
| Blocked         |            0 |
| Not Executed    |            0 |
| **Total** | **28** |

### Result Distribution

* **Passed:** 78.6%
* **Failed:** 21.4%
* **Blocked:** 0%

## 4. Failed Test Cases

The following test cases were affected by identified defects:

| Test Case | Result | Related Bug |
| --------- | ------ | ----------- |
| TC-006    | Failed | BR-005      |
| TC-010    | Failed | BR-001      |
| TC-013    | Failed | BR-002      |
| TC-015    | Failed | BR-003      |
| TC-018    | Failed | BR-004      |
| TC-024    | Failed | BR-006      |

## 5. Defects Summary

A total of **6 defects** were documented.

| Bug ID | Severity | Priority | Status |
| ------ | -------- | -------- | ------ |
| BR-001 | High     | High     | Open   |
| BR-002 | High     | High     | Open   |
| BR-003 | High     | High     | Open   |
| BR-004 | Critical | High     | Open   |
| BR-005 | Medium   | Medium   | Open   |
| BR-006 | Medium   | High     | Open   |

## 6. Testing Results by Area

| Test Area         | Result | Related Test Cases |
| ----------------- | ------ | ------------------ |
| Login             | Passed | TC-001–TC-004     |
| Products          | Failed | TC-005–TC-009     |
| Product Details   | Failed | TC-010–TC-012     |
| Product Sorting   | Failed | TC-006–TC-009     |
| Shopping Cart     | Failed | TC-013–TC-016     |
| Checkout          | Failed | TC-017–TC-021     |
| Checkout Overview | Passed | TC-022–TC-023     |
| Order Completion  | Failed | TC-024–TC-025     |
| Navigation        | Passed | TC-026             |
| Logout            | Passed | TC-027–TC-028     |

### Area Status Rationale

* **Products — Failed:** TC-006 failed because product sorting did not work correctly.
* **Product Details — Failed:** TC-010 failed because incorrect product information was displayed.
* **Product Sorting — Failed:** TC-006 failed due to incorrect sorting behavior.
* **Shopping Cart — Failed:** TC-013 and TC-015 failed due to add/remove cart defects.
* **Checkout — Failed:** TC-018 failed because the Last Name field did not behave correctly.
* **Checkout Overview — Passed:** TC-022 and TC-023 passed.
* **Order Completion — Failed:** TC-024 failed because checkout could be completed with an empty cart.
* **Login — Passed:** TC-001–TC-004 passed.
* **Navigation — Passed:** TC-026 passed.
* **Logout — Passed:** TC-027–TC-028 passed.

## 7. Major Findings

The main issues identified during testing were related to:

* Incorrect product information for the affected test account.
* Product add-to-cart functionality.
* Product removal from the shopping cart.
* Checkout form input.
* Product sorting.
* Checkout with an empty cart.

The most critical documented defect is **BR-004**, which affects the checkout flow.

## 8. Conclusion

The main user flow of the application is functional, but several defects were identified during testing.

Critical and high-priority defects should be addressed before the affected functionality is considered ready for release.

Regression testing should be performed after the defects are fixed to verify that the affected functionality works as expected and that no new issues have been introduced.

## 9. Final Status

**Testing Status:** Completed

**Overall Result:** Failed

**Recommendation:** Fix critical and high-priority defects and perform regression testing before release.
