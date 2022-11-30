---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.People

$params = @{
	Categories = @(
		"Professional"
	)
	AllowedAudiences = "organization"
	DisplayName = "API Design"
	Proficiency = "generalProfessional"
	CollaborationTags = @(
		"ableToMentor"
	)
}

# A UPN can also be used as -UserId.
New-MgUserProfileSkill -UserId $userId -BodyParameter $params

```