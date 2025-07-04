# Test Case 2: Retrieve User Information

## Objective
To validate that specific user information can be accurately retrieved from the users table based on user ID.
## Pre-requisites
- The users table must be created and populated with test data.
- PostgreSQL database must be running.
- Python environment with SQLAlchemy installed.
## Test Steps
1. Establish Database Connection:
- Connect to the PostgreSQL database using SQLAlchemy.
2. Define Query:
- Create a SQL query to retrieve user information based on a specific user ID (e.g., user_id = 2).
3. Execute Query:
- Provide the specific user ID (e.g., 2) and execute the query.
4. Fetch Results:
- Retrieve the result of the query.
5. Validate Results:
- Check if the returned user information matches the expected data for user ID 2:
## Expected Result
The query should return a single record matching the criteria:
## Actual Result
The query returned a single record matching the criteria
## Post-conditions
Ensure the database remains unchanged after the test execution.
## Cleanup
Close the database connection.
## Status
PASS
