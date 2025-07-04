# Test Case 3: Finding Users with NULL Email

## Objective
To verify that the database can accurately retrieve users who have not provided an email address (i.e., users with NULL email).
## Pre-requisites
- The users table must be created and populated with test data.
- PostgreSQL database must be running.
- Python environment with SQLAlchemy installed.
## Test Steps
1. Establish Database Connection:
- Connect to the PostgreSQL database using SQLAlchemy.
2. Define Query:
- Create a SQL query to retrieve users with NULL email addresses.
3. Execute Query:
- Execute the query to retrieve users with NULL email.
4. Fetch Results:
- Retrieve the results of the query.
5. Validate Results:
- Check if the number of returned records matches the expected count.
6. Verify that each returned record matches the expected data:
## Expected Result
The query should return all records with no email address:
## Actual Result
All records with no email address were returned.
## Post-conditions
Ensure the database remains unchanged after the test execution.
### Cleanup
Close the database connection.
## Status
PASS
