# Test Case 1: Query All Data from Database

## Objective
To verify that all user data present in the users table can be successfully queried.
## Pre-requisites
- The users table must be created and populated with test data.
- PostgreSQL database must be running.
- Python environment with SQLAlchemy installed.
## Test Steps
1. Establish Database Connection:
- Connect to the PostgreSQL database using SQLAlchemy.
2. Define Query:
- Create a SQL query to retrieve all records from the users table.
3. Execute Query:
- Execute the query to retrieve all user data.
4. Fetch Results:
- Retrieve the results of the query.
5. Validate Results:
- Check if the number of returned records matches the expected count (8).
6. Verify that each user record matches the expected data:
- User ID, Username, Email, and Status for all entries.
## Expected Result
The query should return all records from the users table, matching the expected data.
## Actual Result
The query returned all records from the users table, matching the expected data.
## Post-conditions
Ensure the database remains unchanged after the test execution.
## Cleanup
Close the database connection.
## Status
PASS
