---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Devices.CorporateManagement

$params = @{
	"@odata.type" = "#microsoft.graph.managedDeviceMobileAppConfigurationUserSummary"
	pendingCount = 12
	notApplicableCount = 2
	successCount = 12
	errorCount = 10
	failedCount = 11
	lastUpdateDateTime = [System.DateTime]::Parse("2016-12-31T23:58:21.6459442-08:00")
	configurationVersion = 4
}

Update-MgDeviceAppMgtMobileAppConfigurationUserStatusSummary -ManagedDeviceMobileAppConfigurationId $managedDeviceMobileAppConfigurationId -BodyParameter $params

```