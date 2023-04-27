---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	extensionAttributes = @{
		extensionAttribute1 = "BYOD-Device"
	}
}

Update-MgBetaDevice -DeviceId $deviceId -BodyParameter $params

```