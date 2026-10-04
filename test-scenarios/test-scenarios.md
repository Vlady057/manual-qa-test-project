
# Test Scenarios

## 1. Login

| ID     | Test Scenario                                 |
| ------ | --------------------------------------------- |
| TS-001 | Verify login with valid credentials           |
| TS-002 | Verify login with invalid username            |
| TS-003 | Verify login with invalid password            |
| TS-004 | Verify login with empty username              |
| TS-005 | Verify login with empty password              |
| TS-006 | Verify login with empty username and password |

## 2. Products

| ID     | Test Scenario                                        |
| ------ | ---------------------------------------------------- |
| TS-007 | Verify products are displayed after successful login |
| TS-008 | Verify product names are displayed correctly         |
| TS-009 | Verify product prices are displayed                  |
| TS-010 | Verify product images are displayed                  |
| TS-011 | Verify products can be sorted by name A-Z            |
| TS-012 | Verify products can be sorted by name Z-A            |
| TS-013 | Verify products can be sorted by price low to high   |
| TS-014 | Verify products can be sorted by price high to low   |

## 3. Product Details

| ID     | Test Scenario                                                |
| ------ | ------------------------------------------------------------ |
| TS-015 | Verify product details can be opened                         |
| TS-016 | Verify product name is displayed on the product details page |
| TS-017 | Verify product description is displayed                      |
| TS-018 | Verify product price is displayed                            |
| TS-019 | Verify product image is displayed                            |
| TS-020 | Verify user can return to the products page                  |

## 4. Shopping Cart

| ID     | Test Scenario                                        |
| ------ | ---------------------------------------------------- |
| TS-021 | Verify a product can be added to the cart            |
| TS-022 | Verify multiple products can be added to the cart    |
| TS-023 | Verify the cart displays added products              |
| TS-024 | Verify product quantity is displayed correctly       |
| TS-025 | Verify a product can be removed from the cart        |
| TS-026 | Verify the cart is empty after removing all products |
| TS-027 | Verify user can continue shopping from the cart      |

## 5. Checkout

| ID     | Test Scenario                                                           |
| ------ | ----------------------------------------------------------------------- |
| TS-028 | Verify checkout can be started from the cart                            |
| TS-029 | Verify checkout form is displayed                                       |
| TS-030 | Verify checkout with valid customer information                         |
| TS-031 | Verify checkout with empty First Name                                   |
| TS-032 | Verify checkout with empty Last Name                                    |
| TS-033 | Verify checkout with empty Zip/Postal Code                              |
| TS-034 | Verify checkout with all required fields empty                          |
| TS-035 | Verify checkout information is displayed correctly on the overview page |

## 6. Order Completion

| ID     | Test Scenario                                                             |
| ------ | ------------------------------------------------------------------------- |
| TS-036 | Verify order total is calculated correctly                                |
| TS-037 | Verify user can complete an order                                         |
| TS-038 | Verify order confirmation is displayed after successful checkout          |
| TS-039 | Verify completed order returns the user to the expected application state |

## 7. Navigation and Logout

| ID     | Test Scenario                                                                     |
| ------ | --------------------------------------------------------------------------------- |
| TS-040 | Verify navigation menu can be opened                                              |
| TS-041 | Verify user can log out                                                           |
| TS-042 | Verify logged-out user cannot access authenticated pages without logging in again |
