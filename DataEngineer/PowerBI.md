Advanced tecniques for users who have mastered the basics

##Power BI navigation - Navigation has quite a bit of impact on use adoption.  

[Apps support customized navigation](https://powerbi.microsoft.com/en-us/blog/designing-custom-navigation-for-power-bi-apps-is-now-available/)

[Button navigation - Actions](https://radacad.com/page-navigation-buttons-in-power-bi)

[Bookmarks - Storytelling](https://docs.microsoft.com/en-us/power-bi/create-reports/desktop-bookmarks) and some [Use case examples](https://tessellationtech.io/toggling-views-with-bookmarks-in-power-bi/) 

[Drill to page](https://docs.microsoft.com/en-us/power-bi/create-reports/desktop-drillthrough) and [Drill buttons](https://docs.microsoft.com/en-us/power-bi/create-reports/desktop-drill-through-buttons) and some [Walk through](https://www.wallstreetmojo.com/power-bi-drill-through/) 

[Cross drill - drill to new report](https://docs.microsoft.com/en-us/power-bi/create-reports/desktop-cross-report-drill-through) and [video walktrough](https://www.youtube.com/watch?v=OcZr_70OGPo&t=4s)


##Data security - restricing access to a subset of the data based on the user
[Basic Row Level Security -RLS](https://docs.microsoft.com/en-us/power-bi/admin/service-admin-rls) and [walk through](https://www.sqlshack.com/introduction-to-row-level-security-in-power-bi/)
Remember that users with RW access to the workspace (Admin, Contributer or Member) will NOT have RLS rules applid.  As editors, they could remove themselves from the role so security is not applied.  It is a best pratice to distribute content via APPs and not the workspaces.  [APPS](https://docs.microsoft.com/en-us/power-bi/consumer/end-user-apps)

For reuse of security rules across Power BI datasets, an approach called Table driven security can be utilized.  This is a more complex technique but makes managment and reuse of rules much easier.  
[Dynamic security](https://radacad.com/dynamic-row-level-security-with-power-bi-made-simple)
[More Dynamic security](https://www.mssqltips.com/sqlservertip/6378/power-bi-table-based-row-level-security/)

Information protection - This is the ability to apply data protection labels so exported content can be secured! 
[Overview of information protection](https://docs.microsoft.com/en-us/power-bi/admin/service-security-data-protection-overview)  This entire section of the document is worth reviewing 
[Video overview](https://www.youtube.com/watch?v=HyfG-0AHdGs)

##Application Lifecycle - Application lifecycle allows you to move PBI content between Development, UAT and Production workspaces.  Think of this as no code devops!  Power BI ALM is a Premium feature.
[Introduction](https://docs.microsoft.com/en-us/power-bi/create-reports/deployment-pipelines-overview)
[Walkthrough](https://visualbi.com/blogs/microsoft/powerbi/application-lifecycle-management-power-bi/)
[Getting started](https://docs.microsoft.com/en-us/power-bi/create-reports/deployment-pipelines-get-started) 

##3rd party tools - Power BI has always been an open and extendable product.  Custom data conntectors and custom visuals have allowed people to extend the product in many new ways.  With Power BI Premium, we have new ways to connect with developer tools.  These are some of the most popular tools.  

While Premium is required to connect to the Power BI service, Premium is not required for use with the Desktop files.  
[Microsofts description](https://powerbi.microsoft.com/en-us/blog/community-tools-for-enterprise-powerbi-and-analysisservices/)

[ALM toolkit](http://alm-toolkit.com/)  Used to compare 2 PBI files or PBI content in the cloud
[Tabular editor free](https://tabulareditor.github.io/) or [commerical license](https://tabulareditor.com/)

[Tabular editor best pratices analyzer](https://guyinacube.com/2021/02/18/best-practice-analyzer-in-tabular-editor-for-your-power-bi-dataset/)  This uses a set of rules to analyze your Power BI data set and idenfifies possible improvments. 

[Dax Studio](https://daxstudio.org/)  If you are writing a lot of Dax this can be a huge asset but it also has the ability to export data, and metadata from your model.  
[Exporting metadata - VPAX files](https://daxstudio.org/documentation/features/model-metrics/)  The file exported is a VPAX file and we can use the 
[Vertipaq Analyzer](https://www.sqlbi.com/tools/vertipaq-analyzer/) to view the data.  See the [walkthrough]()
Or you can view the JSON of the vpax file [Walkthrough](https://www.youtube.com/watch?v=zRa9y01Ub30) 


[So many uses](https://www.oliviertravers.com/power-bi-third-party-tools-development-addons/)

##Calculation groups


##Composite models


##Query Folding



