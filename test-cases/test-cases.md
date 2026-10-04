
# Test Cases

## Login

### TC-001 — Login with valid credentials

**Priority:** High
**Status:** Passed

**Preconditions:** User is on the SauceDemo login page.

**Test Data:**

* Username: `standard_user`
* Password: `secret_sauce`

**Steps:**

1. Enter `standard_user` into the Username field.
2. Enter `secret_sauce` into the Password field.
3. Click **Login**.

**Expected Result:**
User is successfully logged in and redirected to the Products page.

**Actual Result:**
User is redirected to the Products page.

---

### TC-002 — Login with invalid username

**Priority:** High
**Status:** Passed

**Test Data:**

* Username: `invalid_user`
* Password: `secret_sauce`

**Steps:**

1. Enter an invalid username.
2. Enter a valid password.
3. Click **Login**.

**Expected Result:**
An appropriate authentication error message is displayed.

**Actual Result:**
Authentication error is displayed and login is not completed.

---

### TC-003 — Login with invalid password

**Priority:** High
**Status:** Passed

**Test Data:**

* Username: `standard_user`
* Password: `invalid_password`

**Steps:**

1. Enter a valid username.
2. Enter an invalid password.
3. Click **Login**.

**Expected Result:**
An appropriate authentication error message is displayed.

**Actual Result:**
Authentication error is displayed and login is not completed.

---

### TC-004 — Login with empty credentials

**Priority:** High
**Status:** Passed

**Steps:**

1. Leave the Username field empty.
2. Leave the Password field empty.
3. Click **Login**.

**Expected Result:**
Validation message is displayed.

**Actual Result:**
Validation message is displayed.

---

## Products

### TC-005 — Verify product list is displayed

**Priority:** High
**Status:** Passed

**Preconditions:** User is logged in with `standard_user`.

**Steps:**

1. Open the Products page.
2. Review the product list.

**Expected Result:**
Products are displayed with name, image, price, and action button.

**Actual Result:**
Products are displayed correctly.

---

### TC-006 — Sort products by price low to high

**Priority:** High
**Status:** Failed
**Bug:** BR-005

**Preconditions:** User is logged in with `problem_user`.

**Steps:**

1. Open the Products page.
2. Open the sorting dropdown.
3. Select **Price (low to high)**.
4. Review the product order.

**Expected Result:**
Products are sorted from the lowest price to the highest price.

**Actual Result:**
Product order does not correctly correspond to the selected sorting option.

**Bug Report:** `BR-005`

---

### TC-007 — Sort products by price high to low

**Priority:** Medium
**Status:** Passed

**Preconditions:** User is logged in with `standard_user`.

**Steps:**

1. Open the Products page.
2. Select **Price (high to low)**.

**Expected Result:**
Products are sorted from the highest price to the lowest price.

**Actual Result:**
Products are sorted according to the selected option.

---

### TC-008 — Sort products alphabetically A-Z

**Priority:** Medium
**Status:** Passed

**Preconditions:** User is logged in with `standard_user`.

**Steps:**

1. Open the Products page.
2. Select **Name (A to Z)**.

**Expected Result:**
Products are sorted alphabetically from A to Z.

**Actual Result:**
Products are sorted alphabetically from A to Z.

---

### TC-009 — Sort products alphabetically Z-A

**Priority:** Medium
**Status:** Passed

**Preconditions:** User is logged in with `standard_user`.

**Steps:**

1. Open the Products page.
2. Select **Name (Z to A)**.

**Expected Result:**
Products are sorted alphabetically from Z to A.

**Actual Result:**
Products are sorted alphabetically from Z to A.

---

## Product Details

### TC-010 — Verify product images on the Products page

**Priority:** High
**Status:** Failed
**Bug:** BR-001

**Preconditions:** User is logged in with `problem_user`.

**Steps:**

1. Open SauceDemo.
2. Log in with:

   * Username: `problem_user`
   * Password: `secret_sauce`
3. Open the Products page.
4. Review the images displayed for different products.

**Expected Result:**
Each product should display its corresponding product image.

**Actual Result:**
Different products display the same product image instead of their corresponding images.

**Bug Report:** `BR-001`

---

### TC-011 — Verify product details

**Priority:** High
**Status:** Passed

**Preconditions:** User is logged in with `standard_user`.

**Steps:**

1. Open the Products page.
2. Select a product.
3. Review the product details.

**Expected Result:**
Product name, image, description, and price correspond to the selected product.

**Actual Result:**
Product information is displayed correctly.

---

### TC-012 — Return from product details to products

**Priority:** Medium
**Status:** Passed

**Preconditions:** User is viewing product details.

**Steps:**

1. Click **Back to products**.

**Expected Result:**
User is returned to the Products page.

**Actual Result:**
User is returned to the Products page.

---

## Cart

### TC-013 — Add product to cart

**Priority:** High
**Status:** Failed
**Bug:** BR-002

**Preconditions:** User is logged in with `problem_user`.

**Steps:**

1. Open the Products page.
2. Locate **Sauce Labs Bolt T-Shirt**.
3. Click **Add to cart**.

**Expected Result:**
The product is added to the cart and the button changes to **Remove**.

**Actual Result:**
The affected product is not added to the cart as expected.

**Bug Report:** `BR-002`

---

### TC-014 — Add multiple products to cart

**Priority:** High
**Status:** Passed

**Preconditions:** User is logged in with `standard_user`.

**Steps:**

1. Add multiple products to the cart.
2. Open the Cart page.

**Expected Result:**
All selected products are displayed in the cart.

**Actual Result:**
All selected products are displayed in the cart.

---

### TC-015 — Remove product from cart

**Priority:** High
**Status:** Failed
**Bug:** BR-003

**Preconditions:** User is logged in with `problem_user` and has a product in the cart.

**Steps:**

1. Open the Cart page.
2. Click **Remove** for a product.

**Expected Result:**
The selected product is removed from the cart.

**Actual Result:**
The product remains in the cart.

**Bug Report:** `BR-003`

---

### TC-016 — Continue shopping from cart

**Priority:** Medium
**Status:** Passed

**Preconditions:** User is on the Cart page.

**Steps:**

1. Click **Continue Shopping**.

**Expected Result:**
User is returned to the Products page.

**Actual Result:**
User is returned to the Products page.

---

## Checkout

### TC-017 — Open checkout from cart

**Priority:** High
**Status:** Passed

**Preconditions:** User has at least one product in the cart.

**Steps:**

1. Open the Cart page.
2. Click **Checkout**.

**Expected Result:**
Checkout information page is displayed.

**Actual Result:**
Checkout information page is displayed.

---

### TC-018 — Complete checkout information with valid data

**Priority:** High
**Status:** Failed
**Bug:** BR-004

**Preconditions:** User is logged in with `problem_user` and has a product in the cart.

**Test Data:**

* First Name: `Volodymyr`
* Last Name: `QA`
* Zip/Postal Code: `10001`

**Steps:**

1. Open the Cart page.
2. Click **Checkout**.
3. Enter `Volodymyr` into the First Name field.
4. Enter `QA` into the Last Name field.
5. Enter `10001` into the Zip/Postal Code field.
6. Click **Continue**.

**Expected Result:**
All entered values are accepted and the user proceeds to the Checkout Overview page.

**Actual Result:**
The Last Name field does not behave correctly and may place the entered text into the wrong field, preventing normal completion of the checkout form.

**Bug Report:** `BR-004`

---

### TC-019 — Checkout with empty First Name

**Priority:** High
**Status:** Passed

**Preconditions:** User is on the Checkout Information page.

**Steps:**

1. Leave First Name empty.
2. Enter a valid Last Name.
3. Enter a valid ZIP code.
4. Click **Continue**.

**Expected Result:**
Validation message is displayed for the First Name field.

**Actual Result:**
Validation message is displayed.

---

### TC-020 — Checkout with empty Last Name

**Priority:** High
**Status:** Passed

**Preconditions:** User is on the Checkout Information page.

**Steps:**

1. Enter a valid First Name.
2. Leave Last Name empty.
3. Enter a valid ZIP code.
4. Click **Continue**.

**Expected Result:**
Validation message is displayed for the Last Name field.

**Actual Result:**
Validation message is displayed.

---

### TC-021 — Checkout with empty ZIP code

**Priority:** Medium
**Status:** Passed

**Preconditions:** User is on the Checkout Information page.

**Steps:**

1. Enter a valid First Name.
2. Enter a valid Last Name.
3. Leave ZIP code empty.
4. Click **Continue**.

**Expected Result:**
Validation message is displayed for the ZIP code field.

**Actual Result:**
Validation message is displayed.

---

### TC-022 — Verify checkout overview

**Priority:** High
**Status:** Passed

**Preconditions:** User has successfully entered valid checkout information.

**Steps:**

1. Continue to the Checkout Overview page.
2. Review the order information.

**Expected Result:**
Selected products, quantities, prices, subtotal, tax, and total are displayed correctly.

**Actual Result:**
Order information is displayed correctly.

---

### TC-023 — Verify total price calculation

**Priority:** High
**Status:** Passed

**Preconditions:** User is on the Checkout Overview page.

**Steps:**

1. Review product prices.
2. Calculate the expected subtotal.
3. Compare the subtotal, tax, and total with the displayed values.

**Expected Result:**
Displayed subtotal, tax, and total are calculated correctly.

**Actual Result:**
Displayed values are calculated correctly.

---

## Order Completion

### TC-024 — Complete checkout with empty cart

**Priority:** High
**Status:** Failed
**Bug:** BR-006

**Preconditions:** User is logged in with `standard_user`. Cart is empty.

**Test Data:**

* First Name: `Volodymyr`
* Last Name: `QA`
* Zip/Postal Code: `10001`

**Steps:**

1. Open the Cart page without adding any products.
2. Click **Checkout**.
3. Enter valid checkout information.
4. Click **Continue**.
5. Click **Finish**.

**Expected Result:**
The application should prevent checkout when the cart is empty.

**Actual Result:**
The checkout flow can be completed and an order confirmation can be reached without any products.

**Bug Report:** `BR-006`

---

### TC-025 — Verify order confirmation

**Priority:** High
**Status:** Passed

**Preconditions:** User has at least one product in the cart and has completed valid checkout information.

**Steps:**

1. Proceed to the Checkout Overview page.
2. Click **Finish**.

**Expected Result:**
Order confirmation page is displayed.

**Actual Result:**
Order confirmation page is displayed.

---

## Navigation and Logout

### TC-026 — Open navigation menu

**Priority:** Medium
**Status:** Passed

**Preconditions:** User is logged in.

**Steps:**

1. Click the menu button.

**Expected Result:**
Navigation menu is displayed.

**Actual Result:**
Navigation menu is displayed.

---

### TC-027 — Logout

**Priority:** High
**Status:** Passed

**Preconditions:** User is logged in.

**Steps:**

1. Open the navigation menu.
2. Click **Logout**.

**Expected Result:**
User is logged out and redirected to the Login page.

**Actual Result:**
User is redirected to the Login page.

---

### TC-028 — Access protected page after logout

**Priority:** High
**Status:** Passed

**Preconditions:** User has logged out.

**Steps:**

1. Attempt to access the Products page.

**Expected Result:**
Unauthenticated user should not be able to access the protected Products page.

**Actual Result:**
User is redirected to the Login page.
