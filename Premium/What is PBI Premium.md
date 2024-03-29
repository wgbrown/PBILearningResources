Power BI Premium is a capacity-based license that allows for a number of features from unlimited distribution to advanced workloads.
[What is Premium](https://docs.microsoft.com/en-us/power-bi/admin/service-premium-what-is)

Premium is most often used to distribute content (internally or externally) to unlicensed users.  The ability to create new reports remains a Power BI Pro feature.  

**Top reasons to use Premium**

**Unlimited sharing** With Pro licenses, you need to be a Pro user to create or CONSUME a report.  With Premium, anyone (with permission) can consume a report with no per user license.  This includes sharing content to external vendors and partners via [Power BI External Sharing](https://wgbrown.github.io/PBILearningResources/Premium/ExternalSharing)

**Larger data models** - Today PBI Pro supports data models up to 1 gigabyte in space.  While this is highly compressed, there is a limit on the amount of data. With PBI Premium, you can create models as long as they fit into memory (many gigabytes of data).  Design is still critical so refer to the [design documents](https://wgbrown.github.io/PBILearningResources/Data%20Modeling/Modeling.md)  

**More frequent refreshes** - PBI pro supports refreshing your model up to 8 times in 24 hours.  Premium allows unlimited data refreshes.  The UI supports every 30 minutes but with the API you can refresh as often as you like.  [Refresh API](https://powerbi.microsoft.com/en-us/blog/announcing-data-refresh-apis-in-the-power-bi-service/) 

**Life Cycle Management** - Ability to move reports, datasets from Dev to Test to Production workspaces  See [Application LifeCycle](https://wgbrown.github.io/PBILearningResources/DataEngineer/PowerBI)

**Near Real Time Dashboards** - Reports that refresh automatically as data changes when using Direct Query datasets.  While the basic feature is available in Pro, there are advanced settings in Premium.  

**Auto Aggregations** - Data models that use Direct Query can automatically tune themselves to cache frequently used data.  [Auto Aggs](https://learn.microsoft.com/en-us/power-bi/enterprise/aggregations-auto).  Pro also supports user created aggregation tables.  [User created agg tables](https://learn.microsoft.com/en-us/power-bi/transform-model/aggregations-advanced) 

**Pixel Perfect Reports** -  NO LONGER A PREMIUM FEATURE!.  Some reports are best suited to heavily formatted reports.  Often best used for long tables of data or detailed reports from the operational systems.[What are paginated reports](https://docs.microsoft.com/en-us/power-bi/paginated-reports/paginated-reports-report-builder-power-bi) 

**AI integration** - Power Query can access a number of Cognitive services (vision AI) and other ML algorithms

**Monitor performance** - Have insights into the Premium performance [Monitoring App](https://docs.microsoft.com/en-us/power-bi/admin/service-premium-gen2-metrics-app)

**Azure Data Lake integration**- Data flows can easily interoperate with the Azure Data Lake, greatly improving data sharing and access in a secure manner.  [Dataflows and ADL](https://powerbi.microsoft.com/en-us/blog/power-bi-dataflows-and-azure-data-lake-storage-gen2-integration-preview/) 

**XMLA Endpoints** - This opens the full set of pro development tools. See [Third Party Tools](https://wgbrown.github.io/PBILearningResources/DataEngineer/PowerBI) and [Summary](https://powerbi.microsoft.com/en-us/blog/power-bi-open-platform-connectivity-with-xmla-endpoints-public-preview/) 

