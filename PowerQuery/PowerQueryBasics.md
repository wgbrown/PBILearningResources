**Power Query**
[What is Power Query](https://docs.microsoft.com/en-us/power-query/power-query-folding)
Power Query is a core piece of technoligy that is used across many products.

[Documentation](https://docs.microsoft.com/en-us/power-query/)

[Query Folding](https://docs.microsoft.com/en-us/power-query/power-query-folding) can often cause data load performce issues. Many data sources support Power Query to generate
a query against the source database.  Some steps in Power Query can stop the query from being generated and forces Power Query to do all the work!  
It is best to remove any rows of data (filter) and any columns of data (remove columns) before doing anything else.  Most steps can be folded but one example worked as follows:

Steps:
User accessed table of 20 million records (10 year of data)
User added complex converstion of a column (if, then logic)
User removed all but last 3 years of data 

Because the second step (if, then logic) could not be passed down to the database, Power Query returned 20 million rows and then removed all but the last 3 years. 
By reordering steps so the user remove 3 years of data FIRST, Power Query ONLY fetched a smaller subset of data then did the complex converstion.  A refresh than ran several hours,
now runs in 15 minutes.  
