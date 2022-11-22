---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.DeviceManagement.Actions

$params = @{
	UserAccountType = "administrator"
	OsVersion = "windows10"
}

Invoke-MgReprovisionDeviceManagementVirtualEndpointCloudPc -CloudPCId $cloudPCId -BodyParameter $params

```