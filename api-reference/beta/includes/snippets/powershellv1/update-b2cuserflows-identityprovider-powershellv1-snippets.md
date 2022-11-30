---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	"@odata.id" = "https://graph.microsoft.com/beta/identityProviders/{id}"
}

New-MgIdentityB2CUserFlowIdentityProviderByRef -B2cIdentityUserFlowId $b2cIdentityUserFlowId -BodyParameter $params

```