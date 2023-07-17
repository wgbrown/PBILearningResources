Report optimization focus on data model efficiently, DAX optimizations and report best pratices.  

[Import model optimization](https://docs.microsoft.com/en-us/power-bi/guidance/import-modeling-data-reduction)  The Power BI data models is the starting point for report performance optimization. 
A model that follows best practices often needs no other work on the DAX and report pages.  

[DAX  optimization](https://maqsoftware.com/expertise/powerbi/dax-best-practices#!)  

[Optimization guide](https://docs.microsoft.com/en-us/power-bi/guidance/report-separate-from-model)  This is one part of a larger document. 

[Report page performance analyzer](https://docs.microsoft.com/en-us/power-bi/create-reports/desktop-performance-analyzer) and [Performance Analyzer walk through](https://powerbidocs.com/2019/12/08/power-bi-performance-analyzer/)

[Filters and Slicers](https://askgarth.com/blog/what-are-the-differences-between-a-power-bi-slicer-and-a-filter)  
The Apply All action can greatly improve report performance as well  - now you can set all your slicers before running the report.  [Apply All](https://learn.microsoft.com/en-us/power-bi/create-reports/buttons-apply-all-clear-all-slicers?tabs=powerbi-desktop)

Often the card visual is used to display many KPI values but this can lead to slower performance. [Here is a design option] (https://www.sqlbi.com/articles/optimizing-card-visuals-in-slow-power-bi-reports/)  
Even better is to look at the new [preview Card visual](https://powerbi.microsoft.com/en-us/blog/new-card-visual-public-preview/)

By default, every visual is linked to all other visuals so that one click can result in many queries.  Limiting the interaction between visiuals can improve performance as can limiting the number of visuals on a page. 
[Controlling interactions between visuals] (https://docs.microsoft.com/en-us/power-bi/create-reports/service-reports-visual-interactions)
