---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.DirectoryManagement

$params = @{
	"@odata.id" = "https://graph.microsoft.com/beta/directoryObjects/{id}"
}

New-MgBetaDeviceRegisteredOwnerByRef -DeviceId $deviceId -BodyParameter $params

```