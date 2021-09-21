Creating accurate, fast and useful reports is only part of the job - effective methods of deploying reports is critical for wide adoption.  


[Deployment Whitepaper](https://docs.microsoft.com/en-us/power-bi/guidance/whitepaper-powerbi-enterprise-deployment)<br/>
[Using Apps to distrubute content](https://docs.microsoft.com/en-us/power-bi/consumer/end-user-apps)  See the Data engineer section for using custom navigation with APPs<br/>
[Excel as a client](https://docs.microsoft.com/en-us/power-bi/collaborate-share/service-analyze-in-excel)<br/>
Excel can be an excellent tool for self service analysis - however, there are a few things that need to be done for your data model to be effective.  Power BI has the concept of [implict and explict measures](https://radacad.com/explicit-vs-implicit-dax-measures-in-power-bi).<br/>
Implicit measures are any numeric column is summurize by default.  <br/>
Explicit measures are DAX calculations that summurize data.  <br/>
Excel ONLY understands Explicit measures - so if you want users to be able to use Excel as a tool then make sure you create explict measures!<br/>

While not specificly for a report developer, the adoption framework might be a useful read for a strategy to drive adoption across the organization. [Adoption roadmap](https://docs.microsoft.com/en-us/power-bi/guidance/powerbi-adoption-roadmap-overview)

## Information discovery
Users want to be certain that the reports and datasets they are using have accurate data.  Power BI has the ability for datasets, dataflows, reports and apps to be [Endorsed](https://docs.microsoft.com/en-us/power-bi/collaborate-share/service-endorsement-overview)  

Endorsment has two option: Promoted and Certified
Promoted is the self service model - any report creator can Promote their content.  By promoting it, they are saying that they believe the content to be accurate.
Certified is a managed process. A limited number of users can be assigned this authority.  They have the responsiblity to ensure the quality of the content.  

**Dataset discovery** 
You can help uses discover your data - this helps them get the answers they need without duplicating data or effort.
[Datahub](https://docs.microsoft.com/en-us/power-bi/connect-data/service-datasets-hub)</br>
[Making datasets discoverable](https://docs.microsoft.com/en-us/power-bi/connect-data/service-datasets-hub#make-your-dataset-discoverable)






## Premium feature
Power BI Premium has a deployment feature that allows content to be promoted from a development workspace, to a test workspace and finally a production workspace.  Each step can update connections and parameters.  
[Deployment Pipelines](https://docs.microsoft.com/en-us/power-bi/create-reports/deployment-pipelines-overview)

