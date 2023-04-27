---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	"@odata.type" = "#microsoft.graph.socialIdentityProvider"
	displayName = "Apple"
}

Update-MgIdentityProvider -IdentityProviderBaseId $identityProviderBaseId -BodyParameter $params

```