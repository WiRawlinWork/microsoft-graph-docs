---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.DeviceManagement.Enrolment

$params = @{
	"@odata.type" = "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration"
	displayName = "Display Name value"
	description = "Description value"
	priority = 8
	version = 7
	pinMinimumLength = 
	pinMaximumLength = 
	pinUppercaseCharactersUsage = "required"
	pinLowercaseCharactersUsage = "required"
	pinSpecialCharactersUsage = "required"
	state = "enabled"
	securityDeviceRequired = $true
	unlockWithBiometricsEnabled = $true
	remotePassportEnabled = $true
	pinPreviousBlockCount = 
	pinExpirationInDays = 
	enhancedBiometricsState = "enabled"
}

Update-MgDeviceManagementDeviceEnrollmentConfiguration -DeviceEnrollmentConfigurationId $deviceEnrollmentConfigurationId -BodyParameter $params

```