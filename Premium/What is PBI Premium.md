Power BI Premium is a capacity based license that allows for a number of features from unlimited distribution to advanced workloads.
[What is Premium](https://docs.microsoft.com/en-us/power-bi/admin/service-premium-what-is)

Premium is most often used to distrubute content (internally or externally) to unlicensed users.  The ability to create new reports remains a Power BI Pro feature.  

**Top 10 reason to use Premium**

**Larger data models** - Today PBI Pro supports data models up to 1 gigabyte in space.  While this is highly compressed, there is a limit on the amount of data. With PBI Premium, you can create models as long as they fit into memory (many gigabytes of data).  Design is still critical so refer to the [design documents](https://github.com/wgbrown/PBILearningResources/blob/main/Data%20Modeling/Modeling.md)  

**More frequent refreshes** - PBI pro supports refreshing your model up to 8 times in 24 hours.  Premium allows unlimited data refreshes.  The UI supports every 30 minutes but with the API you can refresh as often as you like.  [Refresh API](https://powerbi.microsoft.com/en-us/blog/announcing-data-refresh-apis-in-the-power-bi-service/) 

**Life Cycle Management** - Ability to move reports, datasets from Dev to Test to Production workspaces  See [Application LifeCycle](https://github.com/wgbrown/PBILearningResources/blob/main/DataEngineer/PowerBI.md)

**Near Real Time Dashboads** - Reports that refresh automaticly as data changes.  This feature applys to Direct Query datasets.  While the basic feature is avaialbe in Pro, there are advanced settings in Premium.  

**Pixel Perfect Reports** -  Some reports are best suited to heavily formatted reports.  Often best used for long tables of data or detailed reports from the operational systems.[What are paginated reports](https://docs.microsoft.com/en-us/power-bi/paginated-reports/paginated-reports-report-builder-power-bi) 

**AI integration** - Power Query can access a number of Cognitivie services (vision AI) and other ML algorithms

**Monitor performance** - Have insights into the Premium performance [Monitoring App](https://docs.microsoft.com/en-us/power-bi/admin/service-premium-gen2-metrics-app)

**Azure Data Lake integration**- Data flows can easily interoperate with the Azure Data Lake, greatly improving data sharing and access in a secure manner.  [Dataflows and ADL](https://powerbi.microsoft.com/en-us/blog/power-bi-dataflows-and-azure-data-lake-storage-gen2-integration-preview/) 

**XMLA Endpoints** - This opens the full set of pro development tools. See [Third Party Tools](https://github.com/wgbrown/PBILearningResources/blob/main/DataEngineer/PowerBI.md) and [Summary](https://powerbi.microsoft.com/en-us/blog/power-bi-open-platform-connectivity-with-xmla-endpoints-public-preview/) 

