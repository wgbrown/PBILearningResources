**Power Query**
[What is Power Query](https://docs.microsoft.com/en-us/power-query/power-query-folding)
Power Query is a core piece of technology that is used across many products.  PQ is a tool to create repeatable process for extracting data and preparing it for use.  

For example, you can remove unneeded data, pivot and unpivot, create new columns and merge data sources in a repeatable process so updating reports is easy.  

[Documentation](https://docs.microsoft.com/en-us/power-query/)

[Walkthrough](https://chandoo.org/wp/power-query-tutorial/)

 
Query Folding can often cause data load performance issues. Many data sources support Power Query to generate a query against the source database.  Some steps in Power Query can stop the query from being generated and forces Power Query to do all the work!  
It is best to remove any rows of data (filter) and any columns of data (remove columns) before doing anything else.  Note that not every data source supports folding!  And not every transformation in Power Query can be folded.  
[Basic Query folding](https://docs.microsoft.com/en-us/power-query/query-folding-basics)<br/>
[Query Folding](https://docs.microsoft.com/en-us/power-query/power-query-folding) 


Most transformational steps can be folded (turned into a query to the source database) but not all transformations.  

One real world example worked as follows:

User accessed table of 20 million records (10 year of data)  
User added complex conversion of a column (if, then logic)  
User removed all but last 3 years of data  

Because the second step (if, then logic) could not be passed down to the database, Power Query returned 20 million rows and then removed all but the last 3 years. 
By reordering steps so the user remove 3 years of data FIRST, Power Query ONLY fetched a smaller subset of data then did the complex column conversion.  A refresh than ran several hours, now runs in 15 minutes.  

**Advanced**
Power Query is a UI for a scripting language so if the UI does not do what you want, then you can leverage a scripting languange for advanced functions
[Power Query M Formula Language](https://docs.microsoft.com/en-us/powerquery-m/)  The language itself is referred to as M.  

[Debugging](https://docs.microsoft.com/en-us/power-query/QueryDiagnostics)

