
# Manual Testing Checklist

## 1. Login

* [ ] Login page is accessible
* [ ] Username field is displayed
* [ ] Password field is displayed
* [ ] Login button is displayed
* [ ] Login with valid credentials works
* [ ] Login with invalid username is rejected
* [ ] Login with invalid password is rejected
* [ ] Login with empty username is rejected
* [ ] Login with empty password is rejected
* [ ] Appropriate error messages are displayed

## 2. Products

* [ ] Products page is displayed after successful login
* [ ] Product names are displayed
* [ ] Product descriptions are available
* [ ] Product prices are displayed
* [ ] Product images are displayed
* [ ] Add to cart buttons are displayed
* [ ] Product sorting dropdown is available
* [ ] Sorting by name A-Z works
* [ ] Sorting by name Z-A works
* [ ] Sorting by price low to high works
* [ ] Sorting by price high to low works

## 3. Product Details

* [ ] Product details page can be opened
* [ ] Product name is displayed
* [ ] Product description is displayed
* [ ] Product price is displayed
* [ ] Product image is displayed
* [ ] Add to cart functionality works
* [ ] Back to products functionality works

## 4. Shopping Cart

* [ ] Product can be added to cart
* [ ] Multiple products can be added
* [ ] Cart icon is updated after adding a product
* [ ] Cart contains the selected products
* [ ] Product name is displayed in the cart
* [ ] Product price is displayed in the cart
* [ ] Product quantity is displayed correctly
* [ ] Product can be removed
* [ ] Cart can become empty after removing products
* [ ] Continue Shopping button works
* [ ] Checkout button works

## 5. Checkout

* [ ] Checkout page can be opened
* [ ] First Name field is displayed
* [ ] Last Name field is displayed
* [ ] Zip/Postal Code field is displayed
* [ ] Checkout with valid information works
* [ ] Empty First Name is rejected
* [ ] Empty Last Name is rejected
* [ ] Empty Zip/Postal Code is rejected
* [ ] Empty required fields are rejected
* [ ] Appropriate validation messages are displayed
* [ ] Cancel/Back navigation works

## 6. Checkout Overview

* [ ] Selected products are displayed
* [ ] Product quantities are correct
* [ ] Product prices are correct
* [ ] Item total is displayed
* [ ] Tax is displayed
* [ ] Final total is displayed
* [ ] Total calculation is correct
* [ ] Finish button is available

## 7. Order Completion

* [ ] Order can be completed
* [ ] Confirmation page is displayed
* [ ] Success message is displayed
* [ ] Order completion information is displayed
* [ ] User can return to the Products page

## 8. Navigation and Logout

* [ ] Navigation menu can be opened
* [ ] All expected menu options are displayed
* [ ] Products navigation works
* [ ] Cart navigation works
* [ ] Logout works
* [ ] User is redirected to the login page after logout
* [ ] Authenticated pages require login after logout

## Checklist Result

| Area                | Result |
| ------------------- | ------ |
| Login               | Passed |
| Products            | Passed |
| Product Details     | Passed |
| Shopping Cart       | Passed |
| Checkout            | Passed |
| Checkout Overview   | Passed |
| Order Completion    | Passed |
| Navigation & Logout | Passed |
