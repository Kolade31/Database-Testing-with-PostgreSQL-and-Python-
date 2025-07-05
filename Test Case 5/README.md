# Test Case 5: Update User Email
## Objective
To verify that a user's email can be successfully updated in the users table.
## Pre-requisites
- The users table must be created and populated with test data.
- PostgreSQL database must be running.
- Python environment with SQLAlchemy installed.
## Test Steps
1. Establish Database Connection:
- Connect to the PostgreSQL database using SQLAlchemy.
2. Initial User Email Verification:
- Query the users table to retrieve the current email for a specific user (e.g., user_id = 1).
3. Define Update Query:
- Create a SQL query to update the user's email for user_id = 1.
4. Execute Update Command:
- Execute the update command.
5. Fetch Updated User Data:
- Query the users table again to verify that the email has been updated.
6. Validate Updated Results:
7. Check if the returned email for user_id = 1 matches the expected updated value:
## Expected Result
The query should return the updated email for user_id = 1
## Status
PASS
## Actual Result
User_id 1 email was successfully updated
## Post-conditions
Ensure the database remains unchanged after the test execution (optional rollback may be performed).
## Cleanup
Close the database connection.
