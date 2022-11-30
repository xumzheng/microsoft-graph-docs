---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Identity.SignIns

$params = @{
	InvitedUserEmailAddress = "admin@fabrikam.com"
	InviteRedirectUrl = "https://myapp.contoso.com"
}

New-MgBetaInvitation -BodyParameter $params

```