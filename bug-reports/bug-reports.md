
# Bug Reports

## BR-001 — Different products display the same image

**Severity:** High
**Priority:** High
**Status:** Open
**Environment:** Windows / Google Chrome
**Test Account:** `problem_user`

### Preconditions

User is logged in with the `problem_user` account.

### Steps to Reproduce

1. Open SauceDemo.
2. Log in with:

   * Username: `problem_user`
   * Password: `secret_sauce`
3. Open the Products page.
4. Review the product images displayed for different products.

### Expected Result

Each product should display its corresponding product image.

### Actual Result

Different products display the same product image instead of their corresponding images.

### Impact

Incorrect product images can mislead users and make it difficult to distinguish between products.

### Notes

The issue is reproducible with the `problem_user` test account.

---

## BR-002 — Some products cannot be added to the cart

**Severity:** High
**Priority:** High
**Status:** Open
**Environment:** Windows / Google Chrome
**Test Account:** `problem_user`

### Preconditions

User is logged in with the `problem_user` account and is on the Products page.

### Steps to Reproduce

1. Open SauceDemo.
2. Log in with:

   * Username: `problem_user`
   * Password: `secret_sauce`
3. Locate **Sauce Labs Bolt T-Shirt**.
4. Click **Add to cart**.
5. Repeat the test with **Sauce Labs Fleece Jacket**.
6. Repeat the test with **Test.allTheThings() T-Shirt (Red)**.

### Expected Result

The selected product should be added to the cart and the button should change to **Remove**.

### Actual Result

The affected products are not added to the cart and the expected button state change does not occur.

### Notes

The issue affects specific products when using the `problem_user` account.

---

## BR-003 — Products cannot be removed from the cart

**Severity:** High
**Priority:** High
**Status:** Open
**Environment:** Windows / Google Chrome
**Test Account:** `problem_user`

### Preconditions

User is logged in with the `problem_user` account and has a product in the cart.

### Steps to Reproduce

1. Open SauceDemo.
2. Log in with:

   * Username: `problem_user`
   * Password: `secret_sauce`
3. Add a product to the cart.
4. Open the Cart page.
5. Click **Remove** for the selected product.

### Expected Result

The selected product should be removed from the cart.

### Actual Result

The product remains in the cart after clicking **Remove**.

### Notes

The issue is reported for specific products under the `problem_user` account.

---

## BR-004 — Last Name field does not accept input during checkout

**Severity:** Critical
**Priority:** High
**Status:** Open
**Environment:** Windows / Google Chrome
**Test Account:** `problem_user`

### Preconditions

User is logged in with the `problem_user` account and has at least one product in the cart.

### Steps to Reproduce

1. Open SauceDemo.
2. Log in with:

   * Username: `problem_user`
   * Password: `secret_sauce`
3. Add a product to the cart.
4. Open the Cart page.
5. Click **Checkout**.
6. Enter `Volodymyr` into the **First Name** field.
7. Click the **Last Name** field.
8. Enter `QA`.

### Expected Result

The entered text should appear in the **Last Name** field.

### Actual Result

The Last Name field does not behave correctly and may place the entered text into the wrong field, preventing normal completion of the checkout form.

### Impact

The defect can block the checkout process for the affected test account.

---

## BR-005 — Product sorting does not work correctly

**Severity:** Medium
**Priority:** Medium
**Status:** Open
**Environment:** Windows / Google Chrome
**Test Account:** `problem_user`

### Preconditions

User is logged in with the `problem_user` account and is on the Products page.

### Steps to Reproduce

1. Open SauceDemo.
2. Log in with:

   * Username: `problem_user`
   * Password: `secret_sauce`
3. Open the product sorting dropdown.
4. Select **Price (low to high)**.
5. Compare the displayed product order.
6. Repeat with **Price (high to low)**.

### Expected Result

Products should be reordered according to the selected sorting option.

### Actual Result

The product order does not change correctly according to the selected sorting option.

### Notes

The issue is specific to the `problem_user` test account.

---

## BR-006 — Checkout can be completed with an empty cart

**Severity:** Medium
**Priority:** High
**Status:** Open
**Environment:** Windows / Google Chrome
**Test Account:** `standard_user`

### Preconditions

User is logged in with the `standard_user` account.

### Steps to Reproduce

1. Open SauceDemo.
2. Log in with:

   * Username: `standard_user`
   * Password: `secret_sauce`
3. Open the Cart page without adding any products.
4. Click **Checkout**.
5. Enter valid checkout information:

   * First Name: `Volodymyr`
   * Last Name: `QA`
   * Zip/Postal Code: `10001`
6. Click **Continue**.
7. Click **Finish**.

### Expected Result

The application should prevent checkout when the cart contains no products and display an appropriate validation message.

### Actual Result

The checkout flow can proceed with an empty cart and an order confirmation can be reached without any products.

### Impact

A user can complete an order flow without purchasing any product.

---

# Bug Report Summary

| Bug ID | Title                                        | Account           | Severity | Priority | Status |
| ------ | -------------------------------------------- | ----------------- | -------- | -------- | ------ |
| BR-001 | Different products display the same image    | `problem_user`  | High     | High     | Open   |
| BR-002 | Some products cannot be added to the cart    | `problem_user`  | High     | High     | Open   |
| BR-003 | Products cannot be removed from the cart     | `problem_user`  | High     | High     | Open   |
| BR-004 | Last Name field does not accept input        | `problem_user`  | Critical | High     | Open   |
| BR-005 | Product sorting does not work correctly      | `problem_user`  | Medium   | Medium   | Open   |
| BR-006 | Checkout can be completed with an empty cart | `standard_user` | Medium   | High     | Open   |

**Total Bugs:** 6
