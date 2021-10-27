Advanced techniques for users who have mastered the basics.  

Pick and choose the topics of interest

**Power BI navigation** - Navigation has quite a bit of impact on use adoption.  

Navigation can be as simple as organizing the reports in an APP to drilling to pages or other reports, or using bookmarks to tell a story with data.  

[Apps support customized navigation](https://powerbi.microsoft.com/en-us/blog/designing-custom-navigation-for-power-bi-apps-is-now-available/)  Apps are a package of reports and dashboards that can be distributed.  Apps have more navigation customization like hiding reports, custom sections and external links.  It is a **best practice** to distribute reports via APPs.  

[Button navigation - Actions](https://radacad.com/page-navigation-buttons-in-power-bi)  Buttons are icons or images that can be placed on a PBI report, these buttons support a number of actions like Q+A, drill through, call a bookmark, etc

[Bookmarks - Storytelling](https://docs.microsoft.com/en-us/power-bi/create-reports/desktop-bookmarks) and some [Use case examples](https://tessellationtech.io/toggling-views-with-bookmarks-in-power-bi/)  Bookmarks are saved report states including filter and slicer selections.  

[Drill to page](https://docs.microsoft.com/en-us/power-bi/create-reports/desktop-drillthrough) and [Drill buttons](https://docs.microsoft.com/en-us/power-bi/create-reports/desktop-drill-through-buttons) and some [Walk through](https://www.wallstreetmojo.com/power-bi-drill-through/)  Drill to page allows you to jump to a new page in the report and pass in your current selection.  Often the target page is hidden, and a navigation button allows for a return back to the originating page.  

[Cross drill - drill to new report](https://docs.microsoft.com/en-us/power-bi/create-reports/desktop-cross-report-drill-through) and [video walkthrough](https://www.youtube.com/watch?v=OcZr_70OGPo&t=4s)  While Drill to page allows a user to jump to another page in the report, cross drill allows the user to jump to a different report.  

[Storytelling resources](https://data-marc.com/2019/07/25/storytelling-with-power-bi-1-7-provide-easy-navigation/) 

**Data security** - Restricting access to a subset of the data based on the user
[Basic Row Level Security -RLS](https://docs.microsoft.com/en-us/power-bi/admin/service-admin-rls) and [walk through](https://www.sqlshack.com/introduction-to-row-level-security-in-power-bi/)  
Remember that users with RW access to the workspace (Admin, Contributor or Member) will NOT have RLS rules applid.  As editors, they could remove themselves from the role so security is not applied.  It is a best practice to distribute content via APPs and not the workspaces.  [APPS](https://docs.microsoft.com/en-us/power-bi/consumer/end-user-apps)

For reuse of security rules across Power BI datasets, an approach called Table driven security can be utilized.  This is a more complex technique but makes management and reuse of rules much easier.  
[Dynamic security](https://radacad.com/dynamic-row-level-security-with-power-bi-made-simple)   
[More Dynamic security](https://www.mssqltips.com/sqlservertip/6378/power-bi-table-based-row-level-security/)

Information protection - This is the ability to apply data protection labels so exported content can be secured! 
[Overview of information protection](https://docs.microsoft.com/en-us/power-bi/admin/service-security-data-protection-overview)  This entire section of the document is worth reviewing 
[Video overview](https://www.youtube.com/watch?v=HyfG-0AHdGs)

**Application Lifecycle** - Application lifecycle allows you to move PBI content between Development, UAT and Production workspaces.  Think of this as no code devops!  Power BI ALM is a Premium feature.
[Introduction](https://docs.microsoft.com/en-us/power-bi/create-reports/deployment-pipelines-overview)
[Walkthrough](https://visualbi.com/blogs/microsoft/powerbi/application-lifecycle-management-power-bi/)
[Getting started](https://docs.microsoft.com/en-us/power-bi/create-reports/deployment-pipelines-get-started) 

**3rd party tools** - Power BI has always been an open and extendable product.  Custom data connectors and custom visuals have allowed people to extend the product in many new ways.  With Power BI Premium, we have new ways to connect with developer tools.  These are some of the most popular tools.  

While Premium is required to connect to the Power BI service, Premium is not required for use with the Desktop files.  
[Microsoft's description](https://powerbi.microsoft.com/en-us/blog/community-tools-for-enterprise-powerbi-and-analysisservices/)

[ALM toolkit](http://alm-toolkit.com/)  Used to compare 2 PBI files or PBI content in the cloud  
[Tabular editor free](https://tabulareditor.github.io/) or [commercial license](https://tabulareditor.com/)

[Tabular editor best practices analyzer](https://guyinacube.com/2021/02/18/best-practice-analyzer-in-tabular-editor-for-your-power-bi-dataset/)  This uses a set of rules to analyze your Power BI data set and identifies possible improvements. 

[Dax Studio](https://daxstudio.org/)  If you are writing a lot of Dax this can be a huge asset but it also has the ability to export data, and metadata from your model.   
[Exporting metadata - VPAX files](https://daxstudio.org/documentation/features/model-metrics/)  The file exported is a VPAX file and we can use the 
[Vertipaq Analyzer](https://www.sqlbi.com/tools/vertipaq-analyzer/) to view the data.  See the [walkthrough](https://www.sqlbi.com/articles/data-model-size-with-vertipaq-analyzer/) and [class](https://www.sqlbi.com/p/dax-tools-video-course/).  Note the class covers several third party tools.

Or you can view the JSON of the vpax file [Walkthrough](https://www.youtube.com/watch?v=zRa9y01Ub30) 

[So many uses](https://www.oliviertravers.com/power-bi-third-party-tools-development-addons/)

**Calculation groups**
Power BI has a powerful calculation language called [DAX](https://wgbrown.github.io/PBILearningResources/Dax/Intro%20To%20Dax).  Often we are required to create the same calculation several times for each metric.  If you have Sales and Returns data, you might have YTD, Last YTD, Prior Month, Year ago for each measure.  

Calculation groups allow you to create a calculation like YTD but apply it to several measures.  

![image](https://user-images.githubusercontent.com/10822387/133331307-547a9ade-f737-485d-a89d-67914235396c.png)

While this is an advanced feature and requires use of a 3rd party tool Tabulear Editor(see above)

[Calculation groups](https://www.sqlbi.com/blog/marco/2020/07/15/creating-calculation-groups-in-power-bi-desktop/) do require a good knowledge of [DAX](https://wgbrown.github.io/PBILearningResources/Dax/Intro%20To%20Dax) 

**Composite models**
Composite models are simply put the ability to mix Imported and Direct Query data, or to mix more than one Direct Query data source in the same model.  
[Overview of Composite models](https://docs.microsoft.com/en-us/power-bi/transform-model/desktop-composite-models)

Composite models open up some wide ranging design options when using Direct Query data models or Live Connections.  

Composite models also support Aggregations - a mix of imported and direct query data in the same dataset.  Aggregates can greatly improve performance on large datasets while leaving all the detail level data available to the users.  

Refer to this section on [data modeling](https://wgbrown.github.io/PBILearningResources/Data%20Modeling/Modeling)

**Query Folding**
Query folding is critical enough and misunderstood enough that it is repeated here.  [See Data modeling section on this](https://wgbrown.github.io/PBILearningResources/PowerQuery/PowerQueryBasics) 
[Detailed walkthrough](https://radacad.com/not-folding-the-black-hole-of-power-query-performance)  
This article mentions "At the time of writing this post Merge Columns doesn’t support Query Folding. I have reported this to Power Query Team, and they are working on it, to solve the issue."  
Power BI and Power Query is under constant development so transformations that don't allow for query folding can and will change.  

[How to determine if Query Folding is happening?](https://www.youtube.com/watch?v=QEFze-LdLqo)


