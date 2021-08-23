# ReplyChallenge

PROBLEM
Reply provides Video Streaming services like sports, movies etc., to their Customers. Before subscribing to their
services customers can register for 15 days free trail account. Before or after completing 15 days free trail they can
make a payment for Annual/Monthly Subscription.
Your solution should be of production quality.
Please Implement below API,
1. Registration service with /users endpoint for taking a JSON body with details such as,
FIELDS & VALIDATIONS

 Username - alphanumeric, no spaces
 Password – min length 8, at least one upper case letter & number
 Email – email id with email format
 DoB (Date of Birth) - ISO 8601 format
 Credit Card Number – This field is optional. If given should have 16 digits.

EXPECTED RESPONSES:

 If the request body fails to satisfy any of the basic validation checks return HTTP Status code: 400
 Reject requests if the user is under the age of 18 and return HTTP Status code: 403
 If the username has already been used reject the request and return HTTP Status code: 409
 A successful action should return HTTP Status code: 201
GET /users endpoint:
Consumer should be able to provide a filter (CreditCard=Yes/No) in his request. If “Yes” then should return Users
registered with Credit Card Number.
If “No” then return Users registered without a Credit Card Number.
Without any filter should return all the Registered Users.

2. Payment service with /payments endpoint for taking a JSON body with details such as,
FIELDS & VALIDATIONS

 Credit Card Number – 16 digits
 Amount – 3 digits
EXPECTED RESPONSES:

 If the request body fails to satisfy any of the basic validation checks return HTTP Status code: 400
 If credit card number is not registered against any Registered User return HTTP Status code: 404
 A successful payment should return HTTP Status code: 201

REQUIREMENTS:
 Use Java and Spring Boot
 Please include instructions for running the application
 We don’t need you to implement any Frontend code
 Use suitable Java Collections to store Users and Payment details. Dont’ use Databases/in-memory Databases
please.
 Your solution should compile successfully.

MAIN TITLE LOREM IPSUM DOLOR SIT ES......2
 Your solution should be of Production quality. Aim of this assignment is to see the quality of the code that you
produce if you were working at Reply.
