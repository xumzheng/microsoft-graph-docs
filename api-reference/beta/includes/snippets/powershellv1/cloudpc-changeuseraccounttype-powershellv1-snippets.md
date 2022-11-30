---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.DeviceManagement.Actions

$params = @{
	UserAccountType = "administrator"
}

Rename-MgDeviceManagementVirtualEndpointCloudPcUserAccountType -CloudPCId $cloudPCId -BodyParameter $params

```