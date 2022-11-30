---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	InvitedUserDisplayName = "John Doe (Tailspin Toys)"
	InvitedUserEmailAddress = "john@tailspintoys.com"
	SendInvitationMessage = $false
	InviteRedirectUrl = "https://myapps.microsoft.com"
}

New-MgInvitation -BodyParameter $params

```