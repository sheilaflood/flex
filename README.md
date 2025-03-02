# flex
○ Your approach to the problem
 I chose to use SQL (snowflake) then did the following: 
	1. Clean up data and convert the string to JSON (using a simple CTE)
	2. Parse the nested JSON so all levels (names & values) are visible 
	3. Validate the results 

○ Any assumptions you made
- Accounts are correctly grouped under appropriate categories (e.g., Flex 2761 is indeed a Bank Account/Current Asset)
- All currencies are the same

○ Any issues or inconsistencies you found in the data
- I added a semicolon to the JSON to get the code to run
- The nested JSON structure was different for assets vs liabilities vs equity. My code should show all categories as long as it follows the primary hierarchical json structure. 

○ What you would do next if you had more time
- I would figure out how to automate the JSON parsing using some kind of cursor or recursive query. I almost missed the last level of asset data (bronze, silver, gold, platinum cards) and I would want to have logic that ensures that doesn’t happen again. 

In order to run my validation script, you should open the SQL file and run each of the validation queries at the bottom of the script (commented section). 

Thanks! 
