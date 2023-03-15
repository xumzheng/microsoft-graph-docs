---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.DeviceManagement.Administration

$params = @{
	"@odata.type" = "#microsoft.graph.cloudPcUserSetting"
	DisplayName = "Example"
	SelfServiceEnabled = $false
	LocalAdminEnabled = $true
	RestorePointSetting = @{
		FrequencyInHours = 16
		UserRestoreEnabled = $true
	}
}

New-MgBetaDeviceManagementVirtualEndpointUserSetting -BodyParameter $params

```