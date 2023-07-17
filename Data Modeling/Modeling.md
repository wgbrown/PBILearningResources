Data modeling is critical to your success.  A good data model should be efficient and easy for users to understand.  This should help jumpstart your knowledge of PBI data modeling.

In Power BI, the dataset is a collection of tables, relationships and calculations making up a model.  Usually Datasets are created to answer a subject matter question and then many reports are created from the dataset.  We often refer to the dataset as a Data Model or Semantic Model. The DataSet is created by connecting to various data sources, renaming fields, removing fields, adding calculated data and otherwise preparing the data for end user. 

A good data model will be smaller, faster and consume less resources. 

This is one small part from the Learn site focused on data modeling.  [Data Model lecture](https://docs.microsoft.com/en-us/learn/modules/model-data-power-bi/)

YouTube lecture on data modeling:  [Data modeling best practices](https://www.youtube.com/watch?v=kiVXI7zjSzY&t=198s) 

Optimization Guide: [Optimization guide](https://docs.microsoft.com/en-us/power-bi/guidance/power-bi-optimization) 

Introduction to Data Modeling (free class): [Class](https://www.sqlbi.com/p/introduction-to-data-modeling-for-power-bi-video-course/)

Best practice Analyzer: [BPA](https://powerbi.microsoft.com/en-us/blog/best-practice-rules-to-improve-your-models-performance/)
BPA is part of the tabular editor - a tool for advanced development of Power BI data models.  It has a paid for [TE3](https://tabulareditor.com/) and a free version [TE2](https://tabulareditor.github.io/TabularEditor/).  Both versions support the Best Practice Analyzer.

BPA is a list of hundreds of rules for Power BI dataset development from dozens of Power BI experts.  You do not need to follow all of the rules, it will spot issues that can impact performance, maintenance and usability.  It is like having a free consultant! 
While Tabular Editor can do a lot more, this is a fantastic free resource.  

While the dataset has the tables, columns and so forth the data does not have to be stored in the tables.  We have Direct Query that allows you to leave the data in the source system but loaded into Power BI on demand.  

Connection types - Power BI supports different methods of connecting to data sources.  
&nbsp;&nbsp;&nbsp;&nbsp;Import:  Data is imported to the in-memory engine and cached there.  
&nbsp;&nbsp;&nbsp;&nbsp;Direct Query:  Data is queried off the data source with each interaction.  
&nbsp;&nbsp;&nbsp;&nbsp;Live:  A connection to a specific database that stores the data and the sematic model.  

If using direct query you are moving the responsibility for performance to the source database.  You might want to ensure that the system can handle the load with increasing the sizes of the servers and tuning the databases.  

[Data sources](https://docs.microsoft.com/en-us/power-bi/connect-data/desktop-data-sources)  
[Connection Types](https://adatis.co.uk/power-bi-connectivity-types/) 

Each connection type has advantages and disadvantages.  To determine which connection type to use, first determine your use case and business requirements.  The most effective is Import mode but often a mix of import and direct query can also be optimal.  This is referred to as [Composite Models](https://docs.microsoft.com/en-us/power-bi/transform-model/desktop-composite-models).  

For very large datasets, composite models support aggregations.  This allows summary data to be in-memory and detail data to remain the data source and seamlessly switch between them.  [Aggregations](https://docs.microsoft.com/en-us/power-bi/transform-model/aggregations-advanced)  
