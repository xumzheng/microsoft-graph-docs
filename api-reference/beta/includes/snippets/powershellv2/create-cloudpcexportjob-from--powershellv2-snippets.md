---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.DeviceManagement.Administration

$params = @{
	reportName = "TotalAggregatedRemoteConnectionReports"
	select = @(
		"CloudPcId"
		"ManagedDeviceName"
		"UserPrincipalName"
		"DaysSinceLastSignIn"
		"TotalUsageInHour"
	)
}

New-MgBetaDeviceManagementVirtualEndpointReportExportJob -BodyParameter $params

```