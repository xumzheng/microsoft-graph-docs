---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	AllowedAudiences = "organization"
	Client = @{
		Department = "Corporate Marketing"
		WebUrl = "https://www.contoso.com"
	}
}

# A UPN can also be used as -UserId.
Update-MgBetaUserProfileProject -UserId $userId -ProjectParticipationId $projectParticipationId -BodyParameter $params

```