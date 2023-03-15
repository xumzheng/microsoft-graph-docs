---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

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
New-MgBetaUserProfileSkill -UserId $userId -BodyParameter $params

```