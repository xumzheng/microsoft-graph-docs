---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Groups

$params = @{
	Values = @(
		@{
			Name = "AllowToAddGuests"
			Value = "true"
		}
	)
}

Update-MgGroupSetting -GroupId $groupId -GroupSettingId $groupSettingId -BodyParameter $params

```