**As a** customer account manager 

**I need** an account microservice with REST API endpoints to create, read, update, delete, and list customer accounts

**So that** customer information can be efficiently managed and accessed by other microservices in the e-commerce platform 
      
### Details and Assumptions
    1. The microservice will manage customer account information.
    2. The service will expose a RESTful API.
    3. Other microservices will consume the API.
    4. Customer data will be stored in a database.
    5. The API should support the following operations:
    6. Create a new customer account
    7. Retrieve a customer account by ID
    8. Update customer account information
    9. Delete a customer account
    10.List all customer accounts
    11.The API responses will use JSON format.
    12.Each customer account will have a unique identifier.      
### Acceptance Criteria     
    gherkin 
    
Scenario: Create a customer account

    Given the customer account service is running
    
    When a valid customer account request is submitted
    
    Then a new customer account should be created successfully

Scenario: Retrieve a customer account

    Given a customer account exists in the system
    When the customer account is requested by ID
    Then the customer account details should be returned

Scenario: Update a customer account

    Given a customer account exists in the system
    When updated customer information is submitted
    Then the customer account information should be updated successfully

Scenario: Delete a customer account

    Given a customer account exists in the system
    When the customer account is deleted
    Then the customer account should be removed from the system

Scenario: List all customer accounts

    Given multiple customer accounts exist in the system
    When all customer accounts are requested
    Then a list of customer accounts should be returned
