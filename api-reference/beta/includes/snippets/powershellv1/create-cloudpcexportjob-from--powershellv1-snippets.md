---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.DeviceManagement.Administration

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

New-MgDeviceManagementVirtualEndpointReportExportJob -BodyParameter $params

```