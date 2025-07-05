# Test Case 7: Violates Foreign Key Constraint
## Objective
To verify that the database correctly enforces foreign key constraints by preventing the deletion of records that are referenced by other tables.
## Pre-requisites
- The users table must be created with a foreign key constraint referencing another table (e.g., roles table).
- The roles table must be populated with valid role IDs.
- PostgreSQL database must be running.
- Python environment with SQLAlchemy installed.
## Test Steps
1. Establish Database Connection:
- Connect to the PostgreSQL database using SQLAlchemy.
2. Identify Foreign Key Constraint:
- Confirm the foreign key relationship, for example, that the role_id in the users table references id in the roles table.
3. Attempt to Delete User:
- Create a SQL query to attempt to delete a user that is currently referenced in another table (e.g., a user with user_id = 1).
4. Validate Exception Handling:
- Check if the appropriate error is raised due to the foreign key constraint violation.
5. Verify Data Integrity:
- Query the users table to confirm that the original records remain unchanged.
## Expected Result
- An exception should be raised indicating a foreign key constraint violation.
- The users table should remain unchanged, containing all original records.
## Status
PASS
## Actual Result
An exception was raised indicating a foreign key violation and the users table remain unchanged.
## Post-conditions
Ensure the database remains unchanged after the test execution.
## Cleanup
Close the database connection.
