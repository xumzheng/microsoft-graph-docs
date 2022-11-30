---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.DeviceManagement.Administration

$params = @{
	"@odata.type" = "#microsoft.graph.cloudPcExternalPartnerSetting"
	EnableConnection = $true
}

Update-MgDeviceManagementVirtualEndpointExternalPartnerSetting -CloudPcExternalPartnerSettingId $cloudPcExternalPartnerSettingId -BodyParameter $params

```