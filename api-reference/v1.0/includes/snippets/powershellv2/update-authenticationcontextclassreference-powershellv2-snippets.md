---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	DisplayName = "Contoso medium"
	Description = "Medium protection level defined for Contoso policy"
	IsAvailable = $true
}

Update-MgIdentityConditionalAccessAuthenticationContextClassReference -AuthenticationContextClassReferenceId $authenticationContextClassReferenceId -BodyParameter $params

```