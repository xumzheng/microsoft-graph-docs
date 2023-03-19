---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.DeviceManagement.Administration

$params = @{
	ReportName = "TotalAggregatedRemoteConnectionReports"
	Select = @(
		"CloudPcId"
		"ManagedDeviceName"
		"UserPrincipalName"
		"DaysSinceLastSignIn"
		"TotalUsageInHour"
	)
}

New-MgBetaDeviceManagementVirtualEndpointReportExportJob -BodyParameter $params

```