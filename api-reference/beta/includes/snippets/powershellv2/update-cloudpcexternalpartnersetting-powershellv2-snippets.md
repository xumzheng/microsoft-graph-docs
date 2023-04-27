---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.DeviceManagement.Administration

$params = @{
	"@odata.type" = "#microsoft.graph.cloudPcExternalPartnerSetting"
	enableConnection = $true
}

Update-MgBetaDeviceManagementVirtualEndpointExternalPartnerSetting -CloudPcExternalPartnerSettingId $cloudPcExternalPartnerSettingId -BodyParameter $params

```