---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
	catalogId = "de9315c1-272b-4905-924b-cc112ca180c7"
	accessPackageResource = @{
		displayName = "Community Outreach"
		description = "https://contoso.sharepoint.com/sites/CSR"
		resourceType = "SharePoint Online Site"
		originId = "https://contoso.sharepoint.com/sites/CSR"
		originSystem = "SharePointOnline"
		accessPackageResourceEnvironment = @{
			originId = "https://contoso-admin.sharepoint.com/"
		}
	}
	requestType = "AdminAdd"
}

New-MgEntitlementManagementAccessPackageResourceRequest -BodyParameter $params

```