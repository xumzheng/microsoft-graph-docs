---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	accountEnabled = $false
}

Update-MgBetaDevice -DeviceId $deviceId -BodyParameter $params

```