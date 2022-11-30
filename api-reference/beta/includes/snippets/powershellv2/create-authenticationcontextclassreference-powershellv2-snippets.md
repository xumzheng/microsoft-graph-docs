---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	Id = "c1"
	DisplayName = "Contoso medium"
	Description = "Medium protection level defined for Contoso policy"
	IsAvailable = $true
}

New-MgBetaIdentityConditionalAccessAuthenticationContextClassReference -BodyParameter $params

```