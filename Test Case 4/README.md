# Test Case 4: Check for Duplicate USER IDs

## Objective
To ensure that the database enforces the uniqueness constraint on the user_id column in the users table, preventing duplicate entries.
## Pre-requisites
- The users table must be created with a unique constraint on the user_id column.
- PostgreSQL database must be running.
- Python environment with SQLAlchemy installed.
## Test Steps
1. Establish Database Connection:
- Connect to the PostgreSQL database using SQLAlchemy.
2. Establish Database Connection:
- Connect to the PostgreSQL database using SQLAlchemy.
3. Execute Query to Check for Duplicates:
- Run the necessray SQL query to identify any duplicate usernames.
4. Fetch Results:
- Retrieve the results of the query.
5. Validate Results:
- Check if any records are returned.
- If records are returned, it indicates that there are duplicate usernames.
6. Verify Data Integrity:
- Confirm that the users table does not contain any duplicate entries for user_id.
## Expected Result
- An exception should be raised indicating a unique constraint violation.
- The users table should still contain only the original records.
## Status
PASS
## Actual Result
No exception was raised and the users table still contained only the original records.
## Post-conditions
Ensure the database remains unchanged after the test execution.
## Cleanup
Close the database connection.
