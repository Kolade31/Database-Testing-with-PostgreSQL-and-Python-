# Test Case 6: Finding Invalid Statuses
## Objective
To verify that the database can accurately identify users with invalid statuses in the users table.
## Pre-requisites
- The users table must be created and populated with test data, including a mix of valid and invalid statuses.
- PostgreSQL database must be running.
- Python environment with SQLAlchemy installed.
## Test Steps
1. Establish Database Connection:
- Connect to the PostgreSQL database using SQLAlchemy.
2. Define Query for Invalid Statuses:
- Create a SQL query to find users with statuses that are not in the predefined list of valid statuses (e.g., 'Active', 'Blocked', 'Inactive').
3. Execute Query:
- Execute the query to retrieve users with invalid statuses.
4. Fetch Results:
- Retrieve the results of the query.
5. Validate Results:
- Check if the returned records contain users with invalid statuses.
- Verify the expected invalid statuses against the actual results.
## Expected Result
The query should return users with invalid statuses.
## Status
PASS
## Actual Result
Users with invalid statuses are returned and if none exists a message indicating that shows.
## Post-conditions
Ensure the database remains unchanged after the test execution.
## Cleanup
Close the database connection.
