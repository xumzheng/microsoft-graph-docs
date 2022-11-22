---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.People

$params = @{
	Categories = @(
		"Professional"
	)
	Proficiency = "advancedProfessional"
}

# A UPN can also be used as -UserId.
Update-MgBetaUserProfileSkill -UserId $userId -SkillProficiencyId $skillProficiencyId -BodyParameter $params

```