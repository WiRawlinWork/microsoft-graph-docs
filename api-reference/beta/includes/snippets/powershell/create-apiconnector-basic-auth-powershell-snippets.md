---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	displayName = "Test API"
	targetUrl = "https://someapi.com/api"
	authenticationConfiguration = @{
		"@odata.type" = "#microsoft.graph.basicAuthentication"
		username = "<USERNAME>"
		password = "<PASSWORD>"
	}
}

New-MgIdentityApiConnector -BodyParameter $params

```