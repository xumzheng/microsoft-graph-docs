---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Applications

$params = @{
	"@odata.id" = "https://graph.microsoft.com/v1.0/directoryObjects/{id}"
}

New-MgServicePrincipalOwnerByRef -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```