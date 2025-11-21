# 🧪 AutomationExercise API Testing Collection

**This repository contains a Postman Collection designed to validate multiple API endpoints of the AutomationExercise`[https://automationexercise.com/]` platform.
The project covers both positive and negative scenarios across product listings, brand listings, authentication, user account management, and product search functionalities.**

# 📘 Project Overview

The objective of this project is to verify the functional behavior of publicly available APIs from AutomationExercise.com using Postman.

**The collection includes structured test cases for the following:**

    ~Product list retrieval

    ~Brand list retrieval

    ~Login verification (positive and negative)
  
    ~User account creation, update, and deletion

    ~Fetching user details by email

    ~Product search functionality

All requests are grouped by feature for clear navigation and improved test coverage.

# 📂 Collection Structure
*1. Products List*

GET `/api/productsList` – Retrieve all available products

POST `/api/productsList` – Negative test (invalid method)

GET `/view_cart?ajax=true` – View items in the cart

*2. Brands List*

**GET** `/api/brandsList` – Retrieve all brands

**PUT** `/api/brandsList` – Negative test (invalid method)

*3. Verify Login*

**POST** `/api/verifyLogin` – Missing parameters test

**DELETE** `/api/verifyLogin`– Invalid method test

**POST** `/api/verifyLogin` – Test with invalid credentials

**POST** `/api/verifyLogin` – Test with valid credentials (if the account exists)

*4. User Account Management*

**POST** `/api/createAccount` – Create a new user

**PUT** `/api/updateAccount` – Update existing user

**DELETE** `/api/deleteAccount` – Delete user account

**GET** `/api/getUserDetailByEmail?email=` – Fetch user details by email

*5. Search Products*

**POST** `/api/searchProduct` – Valid product search

**POST** `/api/searchProduct` – Missing parameter negative test

# 🛠️ How to Use This Collection

-> Install Postman

-> Import the collection JSON file

-> Configure baseURL (optional, default is empty)

-> Execute individual requests or run full test sets

-> Validate:

      -Status codes

      -Response messages

      -Error responses

      -Payload structure

# ✔️ Test Scenarios Covered
**Positive Tests**

~Successful login

~Successful account creation

~Valid product searches

~Retrieving full product list

~Retrieving brand list

~Fetching user details by email

**Negative Tests**

~Missing required parameters

~Invalid HTTP method usage

~Invalid login credentials

~Incorrect search parameters

~Empty delete account parameters

# 🧰 Tools Used

>Postman – API testing

>JSON – Request/response formatting

>AutomationExercise Public APIs – Test environment

# 📌 Notes

>This project uses publicly available APIs designed for learning and testing.

>No private or sensitive data is stored or used.

>All endpoints are executed directly without modification to server-side behavior.
