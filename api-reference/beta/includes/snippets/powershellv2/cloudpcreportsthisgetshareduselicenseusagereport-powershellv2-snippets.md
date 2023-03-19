---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.DeviceManagement.Actions

$params = @{
	ReportName = "SharedUseLicenseUsageReport"
	Filter = "ServicePlanId eq '2d1d344e-d10c-41bb-953b-b3a47521dca0' and DateTimeUTC gt datetime'2022-11-30'"
	Select = @(
		"ServicePlanId"
		"LicenseCount"
		"ClaimedLicenseCount"
		"DateTimeUTC"
	)
	Skip = 0
	Top = 100
}

Get-MgBetaDeviceManagementVirtualEndpointReportSharedUseLicenseUsageReport -BodyParameter $params

```