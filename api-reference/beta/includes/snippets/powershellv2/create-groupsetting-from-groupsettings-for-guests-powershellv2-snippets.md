---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Groups

$params = @{
	TemplateId = "08d542b9-071f-4e16-94b0-74abb372e3d9"
	Values = @(
		@{
			Name = "AllowToAddGuests"
			Value = "false"
		}
	)
}

New-MgBetaGroupSetting -GroupId $groupId -BodyParameter $params

```