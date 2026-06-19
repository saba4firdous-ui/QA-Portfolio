Bug ID: BUG_101

Title: 
*User is able to cancel an order after it has been shipped*

Module: Order Cancellation

Severity: High

Priority: 
High

# Environment: 
              - OS: macOS
              - Browser: Chrome


# Preconditions:

- User is logged in with valid credentials.
- User has placed an order.
- Order status is "Shipped".

# Steps to Reproduce:

1. Log in to the application.
2. Navigate to Order History.
3. Open the shipped order details.
4. Verify order status is "Shipped".
5. Click the Cancel Order button
6. Confirm cancellation (if prompted).


# Expected Result:

- Order cancellation should not be allowed.
- Appropriate error message should be displayed.
- Order status should remain "Shipped".
- No refund process should be initiated.

# Actual Result:

- Order is cancelled successfully.
- Success message is displayed.
- Order status changes from "Shipped" to "Cancelled".
- Cancellation request is processed despite the order being shipped.


# Status: Open
