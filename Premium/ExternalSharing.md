Organizations often have to share data with vendors and partners.  Power BI allows sharing of live, interactive and secure reports outside of your organization.

**Governance:**
External sharing is a feature that needs to be enabled.  External users are created as Guest users in your Azure AD tenant.  

Your PBI administrator via the [PBI Admin Portal](https://docs.microsoft.com/en-us/power-bi/admin/service-admin-portal) will need to enable "Allow Active Directory guest users to access Power BI" in the Admin portal.  This will allow guest users to view PBI content that has been shared with them after they have been added to Azure AD as a Guest User.

If allowed, users can automatically be added to Azure AD upon first invitation if the setting "Invite external users to your organization" is enabled.  This is known as ad-hoc sharing.  

[Detailed documentation](https://docs.microsoft.com/en-us/power-bi/admin/service-admin-azure-ad-b2b)

[Detailed documentation on PBI external sharing ](https://docs.microsoft.com/en-us/power-bi/guidance/whitepaper-azure-b2b-power-bi) 

Once added reports and Apps can be shared with these users.  One benefit is that if they leave their organization then access to the reports is lost.

Guest users can also have Row Level security applied limiting their access to a subset of data.   See data security section in [Advanced Topics](https://wgbrown.github.io/PBILearningResources/DataEngineer/PowerBI)


