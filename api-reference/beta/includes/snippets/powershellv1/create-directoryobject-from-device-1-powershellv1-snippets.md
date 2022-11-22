---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
	"@odata.id" = "https://graph.microsoft.com/beta/directoryObjects/{id}"
}

New-MgDeviceRegisteredOwnerByRef -DeviceId $deviceId -BodyParameter $params

```