---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
	AccountEnabled = $false
}

Update-MgDevice -DeviceId $deviceId -BodyParameter $params

```