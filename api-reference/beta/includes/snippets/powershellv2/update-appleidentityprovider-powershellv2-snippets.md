---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	"@odata.type" = "#microsoft.graph.socialIdentityProvider"
	DisplayName = "Apple"
}

Update-MgBetaIdentityProvider -IdentityProviderBaseId $identityProviderBaseId -BodyParameter $params

```