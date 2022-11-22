---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	InvitedUserEmailAddress = "admin@fabrikam.com"
	InviteRedirectUrl = "https://myapp.contoso.com"
}

New-MgInvitation -BodyParameter $params

```