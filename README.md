API testing using Postman and Report generation, covering the essential HTTP methods: GET,
POST, PUT, PATCH, and DELETE for a Book Ordering System. Each method is tested to ensure the API endpoints function as expected.

API : https://simple-books-api.glitch.me

Tool Used: Postman, Command Prompt, Newman


1. GET /status
   
Returns the status of the API.

2. GET /books
   
Returns a list of books.

3. GET /books/:bookId
   
Retrieve detailed information about a book.

4. POST /orders
   
Allows you to submit a new order. Requires authentication.

The request body needs to be in JSON format and include the following properties:

• bookId - Integer - Required

• customerName - String - Required

The response body will contain the order Id.

5. GET /orders
    
Allows you to view all orders. Requires authentication.

6. GET /orders/:orderId
    
Allows you to view an existing order. Requires authentication.

7. PATCH /orders/:orderId
    
Update an existing order. Requires authentication.

8. DELETE /orders/:orderId
    
Delete an existing order. Requires authentication.

9. POST /api-clients/
    
To submit or view an order, you need to register your API client.

The request body needs to be in JSON format and include the following properties:

• clientName - String

• clientEmail - String

The response body will contain the access token. The access token is valid for 7 days.
