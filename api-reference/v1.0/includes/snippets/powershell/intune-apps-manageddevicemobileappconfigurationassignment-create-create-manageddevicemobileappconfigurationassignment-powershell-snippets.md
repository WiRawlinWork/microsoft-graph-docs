---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Devices.CorporateManagement

$params = @{
	"@odata.type" = "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment"
	target = @{
		"@odata.type" = "microsoft.graph.allLicensedUsersAssignmentTarget"
	}
}

New-MgDeviceAppMgtMobileAppConfigurationAssignment -ManagedDeviceMobileAppConfigurationId $managedDeviceMobileAppConfigurationId -BodyParameter $params

```