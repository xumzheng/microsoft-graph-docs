---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	"@odata.type" = "#microsoft.graph.socialIdentityProvider"
	ClientSecret = "1111111111111"
}

Update-MgBetaIdentityProvider -IdentityProviderBaseId $identityProviderBaseId -BodyParameter $params

```