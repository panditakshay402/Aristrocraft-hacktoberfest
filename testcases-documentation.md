Aristrocraft:  Test Cases

This document outlines key interactive test cases to ensure functionality, security, and a seamless web flow for Aristrocraft, a premium leather e-commerce website. Each section provides clear steps and expected results for easy understanding by developers and testers alike.

1. User Authentication
Test Case 1.1: User Registration
Steps:
Navigate to the registration page.
Enter valid details (name, email, strong password).
Submit the registration form.
Expected Result:
A success message appears, and the user is redirected to the login page.
Test Case 1.2: Invalid Registration
Steps:

Enter invalid details (incorrect email format, weak password).
Attempt to register.
Expected Result:

The form shows appropriate error messages such as "Invalid email format" or "Password too weak."
Test Case 1.3: User Login
Steps:

Enter valid login credentials (email, password).
Submit the login form.
Expected Result:

User is successfully logged in and redirected to their personalized dashboard.
2. Product Catalog
Test Case 2.1: Product Listing
Steps:

Visit the homepage or product catalog page.
Browse the list of leather products (bags, shoes).
Expected Result:

All products are displayed with correct descriptions, prices, and high-resolution images.
Test Case 2.2: Search and Filter
Steps:

Use the search bar to search for specific products (e.g., "leather bag").
Apply filters (e.g., price range, category).
Expected Result:

The system displays only relevant products based on the search or applied filters.
3. Shopping Cart
Test Case 3.1: Add to Cart
Steps:

Go to the product details page of any item.
Click the "Add to Cart" button.
Expected Result:

The item is added to the cart, and the cart counter is updated.
Test Case 3.2: Update Cart
Steps:

Visit the shopping cart page.
Change the quantity of an item or remove an item from the cart.
Expected Result:

The cart is updated with the new quantity and recalculated total.
4. Payment Integration
Test Case 4.1: Checkout Process
Steps:

Proceed to checkout from the cart page.
Enter valid shipping details and payment information.
Complete the purchase.
Expected Result:

The payment is processed successfully, a confirmation email is sent, and the user is directed to the order confirmation page.
Test Case 4.2: Invalid Payment Handling
Steps:

Enter invalid payment details (e.g., incorrect card number).
Attempt to complete the purchase.
Expected Result:

The payment is declined, and an error message is shown without completing the purchase.
5. Admin Dashboard
Test Case 5.1: Manage Products
Steps:
Log in to the admin dashboard.
Add, update, or delete a product.
Expected Result:
Product changes are reflected in the product catalog instantly and displayed correctly on the frontend.
6. Vulnerability Testing
Test Case 6.1: SQL Injection
Steps:
Try to inject SQL commands in input fields (e.g., login, search).
Expected Result:
The system securely handles the input, rejecting any harmful SQL commands.
Test Case 6.2: XSS Attack
Steps:

Attempt to inject JavaScript code into input fields (e.g., product reviews, search).
Expected Result:

The input is sanitized, preventing any script from executing.
Test Case 6.3: CSRF Protection
Steps:

Simulate a CSRF attack by sending a malicious request.
Expected Result:

The request is blocked, and no actions are performed.
7. Correct Web Flow Testing
Test Case 7.1: Home Page to Product Details
Steps:

Navigate from the home page to the product catalog.
Select a product to view its details.
Expected Result:

The user flows seamlessly from the home page -> product catalog -> product details.
Test Case 7.2: Product Details to Cart
Steps:

From the product details page, add a product to the cart.
Proceed to the cart view.
Expected Result:

The product is added to the cart, and the user is redirected to the cart page.
Test Case 7.3: Cart to Checkout
Steps:

Proceed to checkout from the cart page.
Complete the purchase.
Expected Result:

The flow from cart -> checkout -> payment -> order confirmation is smooth, with no interruptions.
Test Case 7.4: Login and Checkout
Steps:

Add items to the cart without being logged in.
Attempt to proceed to checkout.
Expected Result:

The user is redirected to the login page, and after logging in, they are brought back to the checkout process.
Note: Perform these tests in a development or staging environment to avoid disrupting live services.

